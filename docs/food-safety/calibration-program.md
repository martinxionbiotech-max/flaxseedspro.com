# Calibration Program

## Document Control

| Field | Value |
|---|---|
| Document ID | FS-CAL-001 |
| Version | 2.1 |
| Effective Date | 2026-01-05 |
| Owner | Maintenance Manager |
| Approver | Food Safety Team Leader |
| Review Frequency | Annual |

---

## 1. Calibration Policy

### 1.1 Purpose
To ensure all measuring, monitoring, and test equipment used for food safety control, quality verification, and process control is calibrated at defined intervals against traceable standards, ensuring accuracy and reliability of results.

### 1.2 Scope
All equipment used in the measurement of parameters critical to food safety and quality, including:
- Temperature (ovens, chillers, freezers, heat exchangers, water heaters)
- Weight / mass (processing scales, checkweighers, lab balances)
- Pressure (CIP pumps, oil presses, steam systems)
- Flow rate (CIP flow meters, ingredient dosing)
- pH (CIP return, water treatment)
- Conductivity / TDS (CIP final rinse, water treatment)
- Humidity (storage areas)
- Metal detection / X-ray (reject verification)
- Time (process timers, cook times)
- Analytical instruments (ELISA readers, ATP luminometers)
- Chemical concentration (dispensers, test kits)

### 1.3 Key Principles
1. **Traceability**: All calibrations must be traceable to national or international standards (NIST, UKAS, ISO 17025 accredited laboratories).
2. **Frequency**: Defined per equipment type (Section 2). Adjust frequency based on drift trends.
3. **Before-use checks**: Operators perform daily verification on critical devices before production start.
4. **Records**: All calibration records retained for minimum 5 years.
5. **Only calibrated equipment** may be used for food safety / quality decisions.
6. **Out-of-tolerance** results trigger formal investigation (Section 4).

### 1.4 Roles & Responsibilities

| Role | Responsibility |
|---|---|
| **Maintenance Manager** | Program owner; schedule execution; external calibration vendor management |
| **QA Manager** | Approval of calibration tolerances; review of out-of-tolerance investigations |
| **Production Operators** | Daily pre-use checks (e.g., checkweigher, metal detector verification) |
| **External Calibration Lab** | Perform annual calibrations with ISO 17025 accredited scope |

---

## 2. Calibration Equipment Register

### 2.1 Master Register

| ID | Equipment | Location | Range / Capacity | Required Accuracy | Standard Used | Frequency | Internal/ External | Procedure Ref |
|---|---|---|---|---|---|---|---|---|
| CAL-T-001 | Oven (Hot Air Dryer) — D-301 | Drying Room | 30–180 °C | ±1.0 °C | Fluke 1523 Reference Thermometer | 6 months | Internal | CAL-PROC-01 |
| CAL-T-002 | Oil Press Heater — H-301 | Oil Press Area | 20–120 °C | ±0.5 °C | Fluke 1523 Reference Thermometer | Monthly (internal) + annual (external) | Both | CAL-PROC-01 |
| CAL-T-003 | Cold Storage — CS-01 | Warehouse | -5 to 10 °C | ±1.0 °C | Pt100 probe + calibrated logger | Monthly (internal) + annual (external) | Both | CAL-PROC-01 |
| CAL-T-004 | Blast Chiller — BC-01 | Packaging Area | -20 to 5 °C | ±1.0 °C | Pt100 probe | Quarterly | Internal | CAL-PROC-01 |
| CAL-T-005 | Steam Boiler Temp Sensor — B-101 | Boiler Room | 100–200 °C | ±2.0 °C | Thermocouple calibrator | Annual | External | CAL-PROC-02 |
| CAL-W-001 | Platform Scale (500 kg) — S-101 | Receiving Bay | 0–500 kg | ±0.1 kg | NIST Class F weights (10 × 20 kg) | Monthly (internal) + annual (external) | Both | CAL-PROC-03 |
| CAL-W-002 | Bench Scale (10 kg) — S-102 | Production Floor | 0–10 kg | ±1 g | NIST Class F weights (1 kg + 5 kg) | Weekly (internal) + annual (external) | Both | CAL-PROC-03 |
| CAL-W-003 | Analytical Balance (220 g) — LB-101 | QA Lab | 0–220 g | ±0.1 mg | NIST Class 1 weights (100 g, 50 g, 20 g) | Quarterly (internal) + annual (external) | Both | CAL-PROC-04 |
| CAL-W-004 | Checkweigher — CW-301 | Packing Line | 0–30 kg | ±5 g | NIST Class F weight set | Daily (auto check) + monthly (internal) + annual (external) | Both | CAL-PROC-03 |
| CAL-P-001 | CIP Supply Pump Pressure Gauge — P-301 | CIP Skid | 0–10 bar | ±0.1 bar | Druck DPI 611 Pressure Calibrator | 6 months | Internal | CAL-PROC-05 |
| CAL-P-002 | Oil Press Hydraulic Gauge — HY-101 | Oil Press | 0–400 bar | ±2 bar | Druck DPI 611 Pressure Calibrator | 6 months | Internal | CAL-PROC-05 |
| CAL-P-003 | Steam Pressure Gauge — ST-101 | Boiler Room | 0–16 bar | ±0.2 bar | Druck DPI 611 Pressure Calibrator | Annual | External | CAL-PROC-06 |
| CAL-F-001 | CIP Flow Meter — FM-301 | CIP Return Line | 0–20 m³/h | ±0.5% of reading | Prover / master meter (tank test) | Annual | External | CAL-PROC-07 |
| CAL-F-002 | Water Flow Meter — FM-201 | Water Inlet | 0–50 m³/h | ±1.0% | Master meter comparison | Biennial | External | CAL-PROC-07 |
| CAL-pH-001 | pH Meter — pH-101 | QA Lab | 0–14 pH | ±0.02 pH | pH buffer standards (pH 4.0, 7.0, 10.0) | Daily (verification) + monthly (full cal) | Internal | CAL-PROC-08 |
| CAL-pH-002 | Inline pH Probe — pH-201 | CIP Return | 0–14 pH | ±0.1 pH | pH buffer loop + lab verification | Weekly (verification) + 6 monthly (full cal) | Both | CAL-PROC-08 |
| CAL-CD-001 | Conductivity Meter — CD-101 | QA Lab | 0–2000 µS/cm | ±1% of reading | KCl conductivity standard (1413 µS/cm) | Monthly | Internal | CAL-PROC-09 |
| CAL-CD-002 | Inline Conductivity Probe — CD-201 | CIP Return | 0–2000 µS/cm | ±2% of reading | KCl standard loop check | Monthly (verification) + annual (full cal) | Both | CAL-PROC-09 |
| CAL-MD-001 | Metal Detector — MD-301 | Packing Line | Ferrous: 0.5–5.0 mm; Non-ferrous: 0.8–5.0 mm; SS: 1.2–5.0 mm | Detects Fe 1.0 mm, NF 1.5 mm, SS 2.0 mm | Calibration test sticks (Fe, NF, SS) | Hourly (run test sticks) + monthly (internal cal) + annual (external) | Both | CAL-PROC-10 |
| CAL-XR-001 | X-ray Inspection — XR-301 | Packing Line | Resolution 0.3 mm | Detects SS 0.5 mm | Calibration test piece (0.5 mm, 1.0 mm SS spheres) | Hourly (run test piece) + monthly (internal) + annual (external) | Both | CAL-PROC-11 |
| CAL-AT-001 | ATP Luminometer — LM-101 | QA Lab | 0–9999 RLU | ±5% at 1000 RLU | ATP calibration standard (provided by manufacturer) | Annual (return to manufacturer) | External | CAL-PROC-12 |
| CAL-AT-002 | ATP Luminometer — LM-102 | Production Floor | 0–9999 RLU | ±5% at 1000 RLU | ATP calibration standard | Annual (return to manufacturer) | External | CAL-PROC-12 |
| CAL-EL-001 | ELISA Plate Reader — EPR-101 | QA Lab | 450 nm, 620/650 nm absorbance | ±0.005 OD | Neutral density filters (0.5, 1.0, 1.5 OD) | Annual | External | CAL-PROC-13 |
| CAL-TI-001 | Process Timer — TIM-101 | Production Line | 0–99 min | ±1 sec | Stopwatch (traceable) | Quarterly | Internal | CAL-PROC-14 |
| CAL-TI-002 | Oven Timer — TIM-201 | Drying Room | 0–99 min | ±5 sec | Stopwatch (traceable) | Quarterly | Internal | CAL-PROC-14 |
| CAL-HU-001 | Humidity Logger — HL-101 | Cold Storage | 20–90% RH | ±3% RH | Humidity generator / saturated salt standards | Annual | External | CAL-PROC-15 |

### 2.2 Colour Coding / Label System
Each calibrated instrument displays a calibration label with:

```
     ┌──────────────────────────┐
     │   CALIBRATION STATUS     │
     │  EQUIPMENT ID: CAL-T-002 │
     │  CAL DATE  : 15/06/2026  │
     │  DUE DATE  : 15/12/2026  │
     │  STATUS  : ✓ IN CAL      │
     │  CAL BY   : Fluke Labs   │
     └──────────────────────────┘
```

- **GREEN** label = In calibration / within due date.
- **RED** label = Out of calibration / past due date. Equipment must NOT be used.
- **YELLOW** label = Calibration due within 30 days (early warning).

---

## 3. Master Standards List

### 3.1 Master Standards with NIST / UKAS Traceability

| Standard ID | Type | Description | Range | Traceability | Calibration Frequency | Custodian |
|---|---|---|---|---|---|---|
| MS-001 | Reference Thermometer | Fluke 1523 w/ PRT probe | -50 to 300 °C | NIST traceable (UKAS certificate) | Annual (external) | QA Lab |
| MS-002 | Temperature Calibrator | Dry-block calibrator (-20 to 150 °C) | -20 to 150 °C | NIST traceable | Annual (external) | Maintenance |
| MS-003 | Mass Standards Set | NIST Class 1 (1 mg – 1 kg) | 1 mg – 1 kg | NIST traceable | Biennial (external) calibration | QA Lab |
| MS-004 | Mass Standards Set | NIST Class F (1 kg – 20 kg × 5) | 1–20 kg (×5) | NIST traceable | Biennial (external) | QA Lab |
| MS-005 | Pressure Calibrator | Druck DPI 611 | 0–400 bar | UKAS traceable | Annual (external) | Maintenance |
| MS-006 | pH Buffers | NIST-traceable buffer solutions (pH 4.0, 7.0, 10.0) | pH 4.0, 7.0, 10.0 | NIST SRM | Monthly (replace solution) | QA Lab |
| MS-007 | Conductivity Standard | KCl solution (1413 µS/cm ±0.5%) | 1413 µS/cm | NIST traceable | Annual (replace) | QA Lab |
| MS-008 | Metal Detector Test Sticks | Fe 1.0 mm, NF 1.5 mm, SS 2.0 mm | Per stated dimensions | Certified by manufacturer | Annual (replace) | QA Lab |
| MS-009 | X-ray Test Piece | SS spheres 0.5 mm, 1.0 mm | Per stated dimensions | Certified by manufacturer | Annual (replace) | QA Lab |
| MS-010 | ATP Calibration Standard | Manufacturer-supplied calibration kit | — | Manufacturer certificate | Annual (replace with kit) | QA Lab |
| MS-011 | Neutral Density Filters | OD 0.5, 1.0, 1.5 | Absorbance | NIST traceable | Biennial | QA Lab |
| MS-012 | Certified Stopwatch | Quartz chronometer traceable to NIST | 0–24 h | NIST traceable | Annual | QA Lab |

### 3.2 Master Standard Usage Rules
1. Master standards are only used for calibration of working instruments — **not** for routine measurements.
2. Master standards are stored in a controlled environment in the QA Lab (20 ± 2 °C, 45 ± 5% RH).
3. Handling requires clean gloves. Standards kept in protective cases when not in use.
4. Any damage or suspected damage to a master standard renders it unusable until re-certification.
5. Log of master standard usage maintained in Master Standard Log (FS-CAL-F01).

---

## 4. Calibration Failure Procedure

### 4.1 Definition
A calibration failure occurs when a calibrated instrument, upon routine calibration, is found to be **outside its required accuracy tolerance**.

### 4.2 Immediate Actions

| Step | Action | Responsible | Timeline |
|---|---|---|---|
| 1 | Tag equipment **OUT OF CALIBRATION** (red label) and remove from service | Calibration Technician | Immediately |
| 2 | Identify all products, batches, or parameters measured by this instrument since its last valid calibration | QA Manager | Within 2 hours |
| 3 | Quarantine affected products / suspend affected process | QA Manager | Within 2 hours |
| 4 | Conduct out-of-tolerance investigation (Section 5) | QA + Maintenance | Within 48 hours |
| 5 | Adjust / repair / replace the instrument | Maintenance / External Lab | As soon as possible |
| 6 | Re-calibrate and return to service with green label | Calibration Technician | After repair |
| 7 | Release or disposition quarantined product based on investigation | Food Safety Team Leader | After investigation |

### 4.3 Quarantine and Product Impact Assessment

The following information must be gathered to assess product impact:

| Data Point | Source |
|---|---|
| Date range of potentially affected measurements | Calibration records (last valid cal date → today) |
| Product lots produced in that date range | Production batch records |
| Critical limits affected (e.g., temperature, weight, metal detection) | HACCP plan / process specs |
| Whether product was already released to customers | ERP / despatch records |
| Customer notification needed? (if product may be unsafe) | Food Safety Team decision |

### 4.4 Escalation
If the calibration failure involves a **CCP monitoring device** (e.g., metal detector, temperature probe in a kill step), escalation to the **Food Safety Team** is mandatory within 2 hours. Regulatory notification may be required if affected product has been released.

---

## 5. Out-of-Tolerance (OOT) Investigation

### 5.1 Investigation Trigger
An OOT investigation is triggered when:
- Calibration result exceeds the specified tolerance.
- Calibration failure is identified during intermediate / daily check (e.g., checkweigher fails daily verification).
- Equipment is found damaged, malfunctioning, or with expired calibration.

### 5.2 Investigation Form (FS-CAL-F02)

**Section A — Incident Details**
| Field | Value |
|---|---|
| Equipment ID | |
| Equipment Description | |
| Parameter measured | |
| Tolerance required | |
| Calibration result (as found) | |
| Date of last valid calibration | |
| Date range possibly affected | |

**Section B — Root Cause Analysis**

Use one of the following methods:
- **5 Whys**: Iterative questioning to find root cause.
- **Fishbone (Ishikawa)**: Categories: Man, Machine, Method, Material, Measurement, Environment.

| Root Cause Factor | Finding |
|---|---|
| Operator error / misuse | |
| Mechanical drift / wear | |
| Environmental conditions (temp, humidity, vibration) | |
| Damage (impact, moisture) | |
| Inadequate calibration frequency | |
| Software / firmware issue | |

**Section C — Product Impact Assessment**

| Question | Answer | Evidence |
|---|---|---|
| Were any products measured during the OOT period? | Y/N | List batches |
| Are any critical limits compromised? | Y/N | Compare readings to CLs |
| Can product risk be quantified? | Y/N | Re-test data |
| Is any product already shipped to customers? | Y/N | Customer list |
| Is customer notification required? | Y/N | Regulatory assessment |

**Section D — Corrective & Preventive Actions (CAPA)**

| Action | Owner | Target Date | Status |
|---|---|---|---|
| Repair / adjust instrument | | | |
| Re-calibrate | | | |
| Re-train operator(s) | | | |
| Adjust calibration frequency | | | |
| Add environmental protection | | | |
| Other | | | |

**Section E — Closure**
| Role | Name | Signature | Date |
|---|---|---|---|
| Investigation Lead | | | |
| QA Manager Review | | | |
| Food Safety Team Leader Approval | | | |

### 5.3 Calibration Frequency Adjustment
Based on OOT investigation findings, the calibration frequency may be adjusted:
- **If drift is minimal and stable**: Frequency may be extended (e.g., from 6 months to 12 months) — requires > 2 years of stable data.
- **If OOT found**: Frequency may be reduced (e.g., from annual to 6 monthly) until stability is demonstrated.
- All frequency changes must be approved by QA Manager and documented on the calibration register.

### 5.4 Trending
Calibration results are trended annually to identify:
- Drift direction / magnitude per instrument type.
- Instruments approaching tolerance limits (predictive calibration).
- Supplier / brand reliability differences.
- Opportunities to extend or need to reduce calibration intervals.

---

## Appendices
- **Appendix A**: Calibration Procedure — Temperature (CAL-PROC-01)
- **Appendix B**: Calibration Procedure — Thermocouple (CAL-PROC-02)
- **Appendix C**: Calibration Procedure — Weights & Scales (CAL-PROC-03)
- **Appendix D**: Calibration Procedure — Analytical Balance (CAL-PROC-04)
- **Appendix E**: Calibration Procedure — Pressure (CAL-PROC-05)
- **Appendix F**: Calibration Procedure — Steam Pressure (CAL-PROC-06)
- **Appendix G**: Calibration Procedure — Flow Meters (CAL-PROC-07)
- **Appendix H**: Calibration Procedure — pH (CAL-PROC-08)
- **Appendix I**: Calibration Procedure — Conductivity (CAL-PROC-09)
- **Appendix J**: Calibration Procedure — Metal Detector (CAL-PROC-10)
- **Appendix K**: Calibration Procedure — X-ray (CAL-PROC-11)
- **Appendix L**: Calibration Procedure — ATP Luminometer (CAL-PROC-12)
- **Appendix M**: Calibration Procedure — ELISA Reader (CAL-PROC-13)
- **Appendix N**: Calibration Procedure — Timers (CAL-PROC-14)
- **Appendix O**: Calibration Procedure — Humidity (CAL-PROC-15)
- **Appendix P**: Master Standard Log (FS-CAL-F01)
- **Appendix Q**: Out-of-Tolerance Investigation Form (FS-CAL-F02)

---

*End of Document — FS-CAL-001*
