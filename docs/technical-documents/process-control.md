# Process Control & Automation System

## 1. SCADA System Overview

The FlaxSeedsPro oil pressing facility is operated through a distributed SCADA (Supervisory Control and Data Acquisition) infrastructure built on **Wonderware System Platform 2023** (now AVEVA™) running on a virtualized Windows Server 2022 environment. The SCADA layer provides real-time process visualization, historian connectivity, alarm management, and supervisory control over all unit operations from seed receiving through oil bottling.

### 1.1 Hardware Architecture

| Component | Specification | Quantity |
|-----------|--------------|----------|
| SCADA Servers (redundant) | Dell PowerEdge R760xs, 2× Xeon Silver 4416+, 128 GB RAM, 2× 1.92 TB SSD RAID-1 | 2 |
| Application Object Server (AOS) | AVEVA System Platform 2023, Galaxy Repository on SQL Server 2022 | 1 |
| Historian Server | AVEVA Historian 2023, 10 TB SAS RAID-10 | 1 |
| HMI Clients | Dell OptiPlex 7080, i7-12700, 32 GB RAM, dual 24" 1920×1080 | 6 |
| Industrial Ethernet Switches | Cisco IE-4010-4S12P, MRP ring topology | 8 |

### 1.2 PLC Platform

The primary process controller is the **Allen-Bradley ControlLogix 5580** (1756-L85E) platform communicating over a redundant ControlNet network with EtherNet/IP bridging to the SCADA layer. Key controller chassis:

| Area | Chassis | CPU | I/O Count | Firmware |
|------|---------|-----|-----------|----------|
| Oil Press Line 1 | CLX-PRESS-01 | 1756-L85E | 256 | v36.011 |
| Solvent Extraction | CLX-SOLV-01 | 1756-L85E | 384 | v36.011 |
| Refining / Bleaching | CLX-REF-01 | 1756-L84ES | 192 | v36.011 |
| Utility Systems (steam, air, water) | CLX-UTIL-01 | 1756-L83E | 128 | v34.014 |

## 2. Control Architecture (ISA-95 / IEC 62264)

The automation system is structured according to the ISA-95 functional hierarchy:

```
Level 4 (ERP)         SAP S/4HANA — Order management, MRP, financials
                          ↑ ↓ (B2MML / XML over HTTPS)
Level 3 (MES)         AVEVA MES 2023 — Batch records, genealogy, OEE, lab data
                          ↑ ↓ (OPC DA / AVEVA OI Gateway)
Level 2 (SCADA)       AVEVA System Platform 2023 — HMI, alarming, trending, historian
                          ↑ ↓ (EtherNet/IP, OPC UA)
Level 1 (PLC/DCS)     Allen-Bradley ControlLogix 5580 / 5380 — Logic, PID, SIF logic solver
                          ↑ ↓ (4-20 mA, RTD, HART, Digital I/O)
Level 0 (Field)       Sensors, actuators, VFDs, analytical instruments, safety sensors
```

### 2.1 Level 0 — Field Instrumentation

All critical process measurements use smart transmitters (Emerson Rosemount 3051S series for pressure/dP/level, and Emerson Rosemount 3144P for temperature) with HART protocol for remote diagnostics. Final control elements include Fisher GX control valves with digital valve controllers (DVC6200) and ABB ACS880 variable frequency drives on all pumps and screw conveyors.

### 2.2 Level 1 — PLC Control

All regulatory control is executed in the ControlLogix processors. PID loops run at 100 ms scan cycles. Safety functions execute in dedicated SIL-rated logic solvers independent of the process controller (see Section 7).

### 2.3 Level 2 — SCADA / HMI

Six HMI workstations provide graphic displays organized by process area. Each display follows EEMUA 191 guidelines: process overview at top, detailed unit graphics with live values, alarm banners, and navigation sidebar. The SCADA system polls all Level 1 controllers at 500 ms intervals for display updates and 1 s for historian collection.

### 2.4 Level 3 — MES

AVEVA MES 2023 manages electronic batch records, material tracking, equipment status, lab sample scheduling, and performance KPIs. MES receives production orders from SAP, disaggregates them into production steps, and returns completed batch dispositions with quality data.

### 2.5 Level 4 — ERP

SAP S/4HANA handles sales order processing, production planning, inventory management, procurement, and financial accounting. Integration to MES uses B2MML (Business-to-Manufacturing Markup Language) over HTTPS with digital signatures for data integrity.

## 3. P&ID Key Elements — Oil Pressing Line

The following control loops are documented in the P&IDs for the mechanical oil pressing line (P&ID drawing set OPL-101 through OPL-120).

### 3.1 Temperature Control Loop TIC-101

- **Service**: Pre-conditioned seed temperature control entering the expeller press
- **Sensor**: RTD Pt-100, 3-wire, Emerson 3144P, range 0–150 °C, accuracy ±0.15 °C
- **Controller**: PID in ControlLogix CLX-PRESS-01, loop update 100 ms
- **Final Element**: Fisher GX 3-inch control valve on steam supply to the seed conditioner jacket
- **Setpoint**: 85 °C (typical), operator adjustable within 65–95 °C
- **Control Strategy**: Cascade from press motor load (master) to jacket temperature (slave)
- **SP Range**: 65–95 °C

### 3.2 Pressure Control Loop PIC-201

- **Service**: Cake discharge back-pressure regulation on expeller press
- **Sensor**: Rosemount 3051S, 0–100 bar, accuracy ±0.04% FS, diaphragm seal
- **Controller**: PID in CLX-PRESS-01, output to hydraulic relief valve
- **Final Element**: Rexroth hydraulic pressure relief valve with proportional solenoid
- **Setpoint**: 65 bar (typical), range 40–90 bar
- **Override**: High-pressure interlock at 95 bar initiates press shutdown sequence

### 3.3 Flow Control Loop FIC-301

- **Service**: Crude oil flow from press collection tank to polishing filter
- **Sensor**: Endress+Hauser Promass F 300 Coriolis mass flow meter, 0–5000 kg/h, ±0.1%
- **Controller**: PID in CLX-PRESS-01, output to VFD speed reference
- **Final Element**: ABB ACS880 VFD on positive-displacement pump P-301
- **Setpoint**: 2500 kg/h (typical), range 500–4000 kg/h

### 3.4 Level Control Loop LIC-401

- **Service**: Crude oil level in intermediate holding tank T-401
- **Sensor**: Rosemount 3051S differential pressure, 0–3000 mmH₂O, remote seal, ±0.065%
- **Controller**: PID in CLX-PRESS-01, output to modulating valve on tank outlet
- **Final Element**: Fisher GX 2-inch globe valve
- **Setpoint**: 50% level (1.5 m), range 10–90%
- **Alarm**: High-high at 85% (tank shutdown), low-low at 10% (pump protection)

## 4. Alarm Management

### 4.1 Alarm Philosophy

The alarm system follows the EEMUA 191 / ISA-18.2 / IEC 62682 standard lifecycle. An Alarm Philosophy Document (APD-001) governs all alarm design, rationalization, and performance monitoring.

### 4.2 Alarm Types

| Category | Definition | Examples |
|----------|-----------|----------|
| **Process Alarms** | Deviations from normal operating range | High temperature, low pressure |
| **Safety Alarms** | Conditions requiring operator intervention to prevent harm | High LEL, high pressure, high temperature |
| **Deviation Alarms** | Deviation of controlled variable from setpoint | PID deviation > 5% for > 30 s |
| **Equipment Alarms** | Asset health warnings | Bearing vibration high, motor overcurrent |
| **System Alarms** | SCADA/network health | PLC communication loss, HART heartbeat fail |
| **Diagnostic Alarms** | Instrument self-diagnostics | Sensor failure, out-of-range signal, calibration overdue |

### 4.3 Priority Levels

| Priority | Color | Annunciation | Max Annunciation Rate | Target Response Time |
|----------|-------|-------------|----------------------|---------------------|
| **High (Priority 1)** | Red | Audible horn + flashing banner | ≤ 2 per hour per operator | ≤ 5 minutes |
| **Medium (Priority 2)** | Amber | Flashing banner | ≤ 10 per hour per operator | ≤ 15 minutes |
| **Low (Priority 3)** | White/Blue | Steady banner or suppressed to alarm log | ≤ 30 per hour per operator | ≤ 60 minutes |

### 4.4 Alarm Rationalization Process

All alarms are subject to a documented rationalization process per ISA-18.2:

1. **Identify** — Master alarm database (MAD) generated from P&ID and HAZOP
2. **Classify** — Assign type, priority, cause, consequence, corrective action
3. **Rationalize** — Multi-discipline review (operations, process engineering, maintenance, HSE)
4. **Apply** — Configure in SCADA and PLC with defined deadbands, on/off delays
5. **Audit** — Annual KPIs: standing alarms ≤ 5, stale alarms ≤ 3, alarm rate peak ≤ 1 per 10 min per operator

### 4.5 Alarm Performance Metrics (Current Year)

| Metric | Actual | Target |
|--------|--------|--------|
| Standing alarms (24-h average) | 3 | ≤ 5 |
| Annunciated alarms per operator per 10 min (peak) | 0.8 | ≤ 1.0 |
| Stale alarms (> 30 days without operator action) | 2 | ≤ 3 |
| Flood duration (> 10 alarms per 10 min) | 0 events/year | 0 |
| Nuisance alarms (bad actors identified per quarter) | 2 | ≤ 5 |

## 5. Batch Tracking and Lot Genealogy

### 5.1 Batch Identification

Each production batch receives a unique 12-character alphanumeric lot code: `YYYYMMDD-LLL-RR` where:
- `YYYYMMDD` = production date
- `LLL` = three-character product code (e.g., `FLO` = Flaxseed Oil, `FOM` = Flaxseed Oil Meal)
- `RR` = two-digit run sequence number

### 5.2 Data Elements Collected Per Batch

| Category | Data Element | Source | Retention |
|----------|-------------|--------|-----------|
| **Identity** | Lot number, product code, batch size (kg), start/end datetime | MES | 10 years |
| **Raw Materials** | Seed lot(s), supplier certificate, quantity, receipt inspection results | MES + SAP | 10 years |
| **Process Parameters** | Temperature profile (TIC-101, 1-min avg), pressure profile (PIC-201), flow (FIC-301), level (LIC-401) | Historian | 10 years |
| **Critical Parameters** | CTP values: max temp, hold time, max pressure | MES | 10 years |
| **Equipment** | Press ID, press speed (rpm), screw configuration | MES | 10 years |
| **Quality** | QC sample results: moisture, protein, ALA, FFA, peroxide value, color | LIMS | 10 years |
| **Operator Entries** | Operator ID, shift, comments (free-text), deviation logs, material additions | MES | 10 years |
| **Events** | Alarm occurrences, overrides, bypasses, manual interventions | Alarm Historian | 10 years |
| **SIF Events** | Safety function actuations, proof test results | SIS Log | 10 years |

### 5.3 Timestamp Synchronization

All data sources are synchronized via NTP to a Stratum-1 GPS time server (Symmetricom TimeProvider 5000). PLC timestamps are accurate to ±10 ms, SCADA historian timestamps to ±100 ms, and MES timestamps to ±1 s.

### 5.4 Lot Genealogy

The MES maintains full **forward and backward traceability** from raw material receipt through to finished product shipment. A genealogy query returns:

- **Upstream**: All raw material lots consumed, equipment IDs, operator IDs
- **Downstream**: All finished product lots produced, pallet IDs, shipment IDs, customer IDs
- **BOM consumption**: Exact quantities (kg) of each material per batch
- **Hold/release status**: Quality disposition at each state (Hold, Released, Rejected, Rework)

Genealogy reports are generated in under 15 s for any lot in the previous 5 years.

## 6. Instrument List (Sample: Oil Pressing Area)

| Tag | Service Description | Type | Range | Accuracy | Location | Cal Freq |
|-----|-------------------|------|-------|----------|----------|----------|
| TT-101 | Seed conditioner outlet temperature | RTD Pt-100, 3-wire | 0–150 °C | ±0.15 °C | Conditioner jacket outlet | 12 months |
| PT-201 | Expeller press cake pressure | Smart dP transmitter, diaphragm seal | 0–100 bar | ±0.04% FS | Press barrel discharge | 6 months |
| FT-301 | Crude oil flow to polishing | Coriolis mass flow | 0–5000 kg/h | ±0.1% | Pipe rack, T-401 outlet | 12 months |
| LT-401 | Crude oil holding tank level | dP with remote seal | 0–3000 mmH₂O | ±0.065% | T-401 bottom nozzle | 12 months |
| AT-501 | Moisture analyzer (NIR) | NIR inline, multi-wavelength | 0–20% H₂O | ±0.1% H₂O | Seed feed chute | 3 months |
| VT-601 | Press motor vibration | Accelerometer, 4–20 mA | 0–50 mm/s | ±0.5 mm/s | Motor DE bearing | 6 months |
| QT-701 | Crude oil FFA (online) | Titration-based analyzer | 0–10% FFA | ±0.05% FFA | Oil line after T-401 | 1 month |
| ST-801 | Seed feed screw speed | Encoder, pulse train | 0–200 rpm | ±0.5 rpm | Screw motor shaft | 12 months |
| ZT-901 | LEL monitor (solvent area) | Catalytic bead | 0–100% LEL | ±2% LEL | Solvent extraction room | 3 months |
| PDT-151 | Polishing filter dP | Smart dP transmitter | 0–5 bar | ±0.04% FS | Filter inlet/outlet | 6 months |

## 7. Safety Instrumented Functions (SIF)

### 7.1 SIF-101: High-Temperature Shutdown — Oil Press

- **SIL Rating**: SIL 2 (required PFDavg < 1×10⁻², achieved PFDavg = 2.1×10⁻³)
- **Function**: On high temperature (> 95 °C) at press barrel, de-energize the press motor VFD and close steam supply valve
- **Sensor**: 2× RTD Pt-100 (TT-101A, TT-101B), 2oo2 voting
- **Logic Solver**: Allen-Bradley GuardLogix 5580 (1756-L85ES), SIL 2 certified
- **Final Element**: Shunt trip on press motor MCC bucket + spring-return steam valve (Fisher GX fail-closed)
- **Proof Test Interval**: 12 months
- **Test Procedure**: SIF-TP-101 — Simulate high temperature using handheld calibrator, verify motor stop and valve travel within 2 s

### 7.2 SIF-201: High LEL — Solvent Extraction

- **SIL Rating**: SIL 2 (required PFDavg < 1×10⁻², achieved PFDavg = 3.4×10⁻³)
- **Function**: On high LEL (> 25% LEL) in solvent extraction area, isolate solvent supply, activate emergency ventilation, and de-energize non-classified electrical equipment
- **Sensor**: 3× catalytic bead LEL sensors (ZT-901A/B/C), 2oo3 voting
- **Logic Solver**: GuardLogix 5580, same chassis as SIF-101 (separate safety task)
- **Final Element**: Solvent supply block valve (ESDV-201), ventilation fan VFD ramp to 100%, MCC shunt trip on non-rated equipment
- **Proof Test Interval**: 6 months
- **Test Procedure**: SIF-TP-201 — Apply calibration gas (50% LEL methane), verify alarms at 10%, isolation at 25%, ventilation start

### 7.3 SIF-301: Emergency Stop — Whole Facility

- **SIL Rating**: SIL 3
- **Function**: One-button facility-wide safe shutdown from any of 12 E-Stop pull-cord stations
- **Note**: This is a hardwired safety function separate from the GuardLogix system, per IEC 60204-1

## 8. Data Historian and Reporting

### 8.1 AVEVA Historian

- **Collection Interval**: 1 s for analog process variables (continuous), event-based for discrete
- **Compression**: Swinging door compression with deadband of 0.5% of range
- **Storage**: 10 TB RAID-10, triple-mirrored for disaster recovery
- **Retention**: All raw data retained for 13 months; aggregated (1-min, 1-hr, 1-day) averages retained for 10 years

### 8.2 Reports

| Report | Frequency | Trigger | Recipients |
|--------|-----------|---------|------------|
| Daily Production Summary | Daily (07:00) | Scheduled | Operations Manager, Shift Supervisors |
| Batch Disposition Report | Per batch | Batch completion | QA Manager, Production Planner |
| Alarm KPI Report | Weekly (Monday) | Scheduled | Operations Manager, Process Engineer |
| SIF Proof Test Status | Monthly | Scheduled | HSE Manager, Maintenance Manager |
| OEE Report | Daily | Scheduled | Plant Manager, Production Manager |
| Utility Consumption | Monthly (1st) | Scheduled | Energy Manager, Plant Controller |
| Deviation / Event Log | On-demand | User request | QA, Process Engineering |

## 9. Recipe Management

### 9.1 Recipe Structure

Recipes are managed in AVEVA MES as **master recipes** (product definitions) that are instantiated as **control recipes** (batch-specific parameter sets). Each master recipe contains:

- **Header**: Product code, recipe version, effective date range, approval status
- **Equipment Requirements**: Primary press ID, filter ID, tank assignment
- **Parameter Set**: All critical process parameters (SP values, ramp rates, hold times, alarm limits)
- **Material BOM**: Raw material types and target quantities per batch
- **Procedure Steps**: Ordered sequence of unit procedures with transitions
- **QC Sampling Plan**: Sampling points, test methods, acceptance criteria

### 9.2 Recipe Parameters per Product

| Parameter | Flaxseed Raw Oil (FLO-01) | Flaxseed Refined Oil (FLO-02) | Flaxseed Meal (FOM-01) |
|-----------|---------------------------|-------------------------------|------------------------|
| Conditioner temp SP | 85 °C | 85 °C | 80 °C |
| Press speed SP | 32 rpm | 32 rpm | 38 rpm |
| Press pressure SP | 65 bar | 65 bar | 55 bar |
| Cake target moisture | N/A | N/A | 8.5% |
| Polishing filter micron | 50 µm | 10 µm | N/A |
| Max oil temp | 90 °C | 90 °C | N/A |
| FFA max (crude) | 2.0% | 1.5% | N/A |

### 9.3 Recipe Change Control

Any modification to a master recipe follows a strict change control workflow:

1. **Initiation** — Request submitted via MES by Process Engineering
2. **Review** — Multi-function review board (operations, quality, process, HSE) within 5 business days
3. **Testing** — Minimum 3 trial batches at proposed settings with full QC analysis
4. **Approval** — Electronic signature by QA Manager and Plant Manager
5. **Version Lock** — Previous recipe version archived (retained indefinitely), new version activated on effective date
6. **Training** — Operators must acknowledge and complete training on recipe changes before first use
7. **Audit Trail** — Full change history maintained including who, what, when, and reason

Recipe version numbers follow the format `V<major>.<minor>` where major versions require full re-validation and minor versions (parameter changes within validated range) require abbreviated verification.

---

*Document reference: PROC-CTL-001 Rev 3.2*
*Last reviewed: 2026-06-15*
*Next review: 2027-06-15*
