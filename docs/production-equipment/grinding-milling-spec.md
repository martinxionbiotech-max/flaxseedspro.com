# Grinding & Milling Equipment — Technical Specification

## 1. Process Objective

Reduce dehulled flaxseed kernels (with or without hull fractions) into controlled particle-size flours and meals at a design capacity of **2 MT/hr max** (typical: 1.2–1.8 MT/hr depending on target fineness). Four milling paths available: hammer mill (coarse), disc mill (medium), pin mill (fine), cryogenic mill (ultra-fine, reduced oxidation).

---

## 2. Equipment Configuration — ASCII Flow Diagram

```
Dehulled kernels / middlings
      |
      v
[ Feed hopper with dosing screw ]          ← VFD-controlled feed rate
      |
      +───→ [ Hammer Mill ]    2,800–3,600 rpm   Screen 0.8–3.0 mm     Coarse meal
      |
      +───→ [ Disc Mill ]      1,200–1,800 rpm   Gap 0.1–2.0 mm        Medium flour
      |
      +───→ [ Pin Mill ]       6,000–12,000 rpm  No screen              Fine flour
      |
      +───→ [ Cryogenic Mill ] −150 °C           1.5–2.5 kg N2/kg      Ultra-fine, cold
                                    ↓                                      ↓
                              Liquid N2 ──→ Exhaust vapour
                                    ↓
                              [ Product cyclone + bag filter ]
                                    ↓
                              [ Metal detector ] ← CCP-2
                                    ↓
                              [ Packing / silo ]
```

---

## 3. Equipment Table

| Unit | Type | Model (Example) | Capacity (MT/hr) | Power (kW) | Material (food-contact) | Manufacturer (suggested) |
|------|------|-----------------|-------------------|------------|------------------------|--------------------------|
| Hammer Mill | Swing-hammer, horizontal shaft, screen basket | Schutte-Buffalo 15-24 | 1.5–2.0 | 37–45 | SS304 chamber, AR400 hammers, SS304 screen | Schutte-Buffalo / Jacobsen |
| Disc Mill | Single/double rotating disc, adjustable gap | Bühler MJZS-80 | 1.0–1.8 | 30–37 | Ni-hard discs, SS304 housing | Bühler / Perten |
| Pin Mill | Vertical, two counter-rotating pin discs | Hosokawa Alpine 160UPZ | 0.5–1.2 | 22–30 | SS316L disc, WC-Co pins | Hosokawa Alpine / Kemutec |
| Cryogenic Mill | Integrated N₂ injection, screw feeder, hammer/impact mill | Air Products / Praxair Cryo-Grind | 0.3–0.8 | 30 (mill) + 15 (N₂ system) | SS304, cryo-rated seals, PTFE gaskets | Air Products / custom |

---

## 4. Detailed Technical Parameters — Set Points & Tolerances

### 4.1 Hammer Mill (2,800–3,600 rpm, 0.8–3.0 mm screen)

| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Rotor speed | 3,200 rpm | ±50 rpm | VFD-controlled |
| Tip speed (rotor Ø 600 mm) | 100 m/s | ±5 m/s | Adjustable via VFD |
| Number of hammers | 24 (4 rows × 6) | — | Reversible (4 wear faces) |
| Hammer thickness | 6 mm | ±0.5 mm | AR400 steel |
| Screen aperture | 1.5 mm | ±0.05 mm | Interchangeable: 0.8 / 1.0 / 1.5 / 2.0 / 3.0 mm |
| Screen open area | 35–45 % | — | Staggered hole pattern |
| Hammer-to-screen clearance | 8 mm | ±1 mm | Critical for grind efficiency |
| Feed rate | 1.5 MT/hr | ±0.2 MT/hr | For 1.5 mm screen |
| Motor full-load amps | 75 A | ±5 A | At 380 V, 50 Hz |
| Product temperature rise | +15 °C max | — | Above ambient |
| Target particle size (d50) | 400 µm | ±50 µm | With 1.5 mm screen |

### 4.2 Disc Mill (1,200–1,800 rpm)

| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Rotating disc speed | 1,500 rpm | ±30 rpm | VFD-controlled |
| Stationary / rotating disc diameter | 300 mm | ±0.5 mm | Ni-hard cast-iron |
| Disc gap (closed) | 0.5 mm | ±0.05 mm | Adjustable by handwheel |
| Disc gap adjustment range | 0.1–2.0 mm | ±0.05 mm | Micrometer dial |
| Groove pattern | Radial, 30° included angle | — | Factory set; re-cut at refurb |
| Feed rate | 1.2 MT/hr | ±0.2 MT/hr | For medium grind |
| Motor power draw (nominal) | 25 kW | ±2 kW | At 1.5 mm gap |
| Product temperature rise | +12 °C max | — | Above ambient |
| Target particle size (d50) | 200 µm | ±30 µm | At 0.5 mm gap |

### 4.3 Pin Mill (6,000–12,000 rpm)

| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Rotor disc speed | 10,000 rpm | ±200 rpm | Belt-driven + VFD |
| Stator disc speed (counter-rotating) | 8,000 rpm | ±200 rpm | Belt-driven + VFD |
| Relative tip speed | 200 m/s | ±10 m/s | Sum of both rotors |
| Number of pins (rotor disc) | 48 | — | WC-Co, Ø 8 mm × 40 mm |
| Number of pins (stator disc) | 48 | — | WC-Co, Ø 8 mm × 40 mm |
| Pin arrangement | 4 concentric rings (staggered) | — | Optimised for flaxseed |
| Feed rate | 0.8 MT/hr | ±0.1 MT/hr | For fine flour |
| Motor power draw (total) | 25 kW | ±3 kW | Both motors combined |
| Product temperature rise | +20 °C max | — | Highest heat of all mills |
| Target particle size (d50) | 80 µm | ±15 µm | For fine bakery flour |
| No-load amps (rotor) | 12 A | ±2 A | Per motor at 380 V |

### 4.4 Cryogenic Mill (−150 °C, N₂ 1.5–2.5 kg N₂/kg)

| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Grinding chamber temperature | −150 °C | ±10 °C | Pt100 RTD, PID-controlled |
| Liquid nitrogen flow rate | 2.0 kg N₂/kg product | ±0.3 kg/kg | Self-regulating valve |
| Product feed rate | 0.5 MT/hr | ±0.1 MT/hr | Max 0.8 MT/hr |
| Product temperature at discharge | −100 °C | ±10 °C | Oil oxidation prevention |
| Nitrogen gas exhaust temperature | +5 °C | ±5 °C | Heat exchanger exit |
| Oxygen in exhaust gas | < 1 % vol | — | Oxygen sensor interlock |
| Mill rotor speed (hammer type) | 3,000 rpm | ±50 rpm | VFD |
| Target particle size (d50) | 30 µm | ±5 µm | Ultra-fine |
| Specific energy | 60 kWh/MT | ±5 kWh/MT | Mill + N₂ production |
| N₂ usage per batch | 1,000 kg N₂/MT | ±150 kg N₂/MT | At 0.5 MT/hr |

---

## 5. Performance Targets & Verification

| Parameter | Target | Verification Method | Frequency |
|-----------|--------|---------------------|-----------|
| Hammer mill — d50 particle size | 400 ± 50 µm (1.5 mm screen) | Sieve analysis (Ro-Tap, 20 min) | Every 2 hr & after screen change |
| Disc mill — d50 particle size | 200 ± 30 µm | Sieve analysis (Ro-Tap, 20 min) | Every 2 hr & after gap adjustment |
| Pin mill — d50 particle size | 80 ± 15 µm | Laser diffraction (Malvern Mastersizer) | Every 4 hr |
| Cryogenic mill — d50 particle size | 30 ± 5 µm | Laser diffraction | Every 4 hr & per batch |
| Throughput (hammer mill) | ≥ 1.5 MT/hr | Belt scale / weigh hopper | Continuous |
| Throughput (cryogenic) | ≥ 0.5 MT/hr | Nitrogen flow integrator | Per batch |
| Product temperature rise | ≤ 20 °C above ambient | IR thermometer at outlet | Hourly |
| Metal detector rejection (CCP-2) | 100 % of ferrous ≥ 1.0 mm, SS ≥ 1.5 mm | Test wands (Fe, SS, Cu) | Start of every shift |
| Specific energy consumption | ≤ 30 kWh/MT (hammer), ≤ 80 kWh/MT (cryo) | Energy meter | Monthly |

---

## 6. HACCP Integration — CCP-2 (Metal Detector)

| Element | Specification |
|---------|--------------|
| **CCP ID** | CCP-2 |
| **Hazard** | Physical — ferrous and non-ferrous metal fragments from mill wear (hammers, pins, discs, screens) |
| **Critical Limit** | Ferrous ≥ 1.0 mm: reject. Stainless steel ≥ 1.5 mm: reject. Non-ferrous (Cu, Al) ≥ 1.5 mm: reject. |
| **Monitoring Device** | In-line metal detector (e.g., Mettler-Toledo Safeline, Thermo Scientific APEX) with auto-eject |
| **Monitoring Frequency** | Continuous production; manual test with test wands every 60 min |
| **Monitoring Personnel** | Line operator |
| **Corrective Action** | 1. Isolate affected product (from last clean test). 2. Reject and quarantine. 3. Investigate source (inspect mill components). 4. Replace worn hammers/pins/screens. 5. Log incident in HACCP record. |
| **Verification** | Third-party metal detector calibration every 6 months; daily shift-start test with Fe/SS/non-Fe wands |
| **Record Keeping** | CCP-2 log (hourly); auto-ejection event log (digital, 90-day retention) |

### Pre-Grinding OPRP — Mill Wear Monitoring

| Equipment | Hazard Controlled | Monitoring | Frequency |
|-----------|-------------------|------------|-----------|
| Hammer mill | Metal fragments from hammer/screen wear | Visual inspection of hammers + screen integrity | Every shift |
| Disc mill | Metal fragments from disc contact | Visual inspection of disc grooves & gap | Every 4 hr |
| Pin mill | Metal fragments from pin fracture | Pin count + visual check | Every 4 hr |
| Cryogenic mill | Metal fragments + seal failure | Visual + oxygen sensor | Every 2 hr |

---

## 7. Maintenance Schedule

### 7.1 Daily (shift-end, ~30 min total)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Hammer mill — inspect hammers for wear/cracks; rotate/replace as needed | 10 | Operator |
| Disc mill — check disc gap; inspect for scoring | 5 | Operator |
| Pin mill — visual pin count (confirm none missing) | 5 | Operator |
| Cryogenic mill — check N₂ line for frost/leaks; verify door seal integrity | 5 | Operator |
| Metal detector — run test wand (Fe, SS, Cu); log result | 5 | Operator |

### 7.2 Weekly (~3 hr)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Hammer mill — measure hammer tip wear (dial calliper); replace if < 80 % original width | 30 | Maintenance tech |
| Hammer mill — rotate hammers to fresh face; replace screen if holes > 110 % of spec | 30 | Maintenance tech |
| Disc mill — remove discs; measure groove depth; dress if < 1 mm remaining | 30 | Maintenance tech |
| Pin mill — remove pin disc; check each pin torque (10 N·m); replace any loose pins | 30 | Maintenance tech |
| Cryogenic mill — check N₂ valve calibration; inspect PTFE seals | 30 | Maintenance tech |
| All mills — lubricate feed screw bearings & shaft seals (food-grade) | 15 | Maintenance tech |
| Metal detector — sensitivity check with all three test pieces | 15 | QC / Tech |
| Cyclone & bag filter — clean; check for wear | 15 | Operator |

### 7.3 Monthly (~6 hr)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Hammer mill — replace all hammers (set of 24); rotate or replace screen basket | 60 | Maintenance team |
| Disc mill — replace discs (both rotors); replace shaft seals | 60 | Maintenance team |
| Pin mill — replace all pins on both discs (96 pins total) | 90 | Maintenance team |
| Cryogenic mill — complete seal replacement (PTFE gaskets, O-rings, shaft seals) | 60 | Maintenance tech + OEM |
| All mills — motor bearing re-grease; shaft alignment check (laser) | 30 | Maintenance tech |
| All mills — VFD parameter backup & firmware check | 15 | Electrical tech |
| Dust collection system — duct inspection; fan bearing replacement (if vibration > 5 mm/s) | 30 | Maintenance tech |
| Full particle-size analysis QC correlation — compare mill lab sieve vs. reference | 15 | QC lab |
| Update spare parts inventory & maintenance log | 15 | Maintenance lead |

### 7.4 Annual (during shutdown, ~24 hr)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Hammer mill — complete rotor refurbishment (re-build shaft, bearings, keyways) | 300 | Maintenance team + OEM |
| Disc mill — complete disc & housing reconditioning; replace all bearings | 240 | Maintenance team |
| Pin mill — complete rotor & stator disc replacement; rebalance both assemblies | 240 | Maintenance team + OEM |
| Cryogenic mill — full overhaul: mill section, N₂ injection nozzles, heat exchanger, control valves | 360 | OEM service engineer |
| All mills — Megger test (all motors > 20 MΩ); motor bearing replacement | 120 | Electrical tech |
| All mills — structural weld inspection; vibration analysis baseline | 60 | Maintenance team |
| Metal detector — factory calibration + report (OEM service) | 60 | OEM service engineer |
| HACCP CCP-2 re-validation — 8-hr challenge test with calibrated test pieces | 240 | QC + Production |

---

## 8. Safety Interlocks & Emergency Stops

| Interlock / E-Stop | Trigger | Action | Location |
|--------------------|---------|--------|----------|
| E-Stop (red pushbutton) | Manual press | Shuts all mill drives + feed screws + dust collection | Each mill panel + line ends |
| Mill door interlock | Access door limit switch | Stops rotor immediately; brake engages (< 5 s stop) | Each mill chamber door |
| Overload relay (motor) | Amperage > 110 % of FLA for 5 s | Trips motor; stops feed | Each motor starter |
| Vibration sensor (mill bearing) | Vibration > 12 mm/s RMS | Trips mill drive | Each bearing housing |
| Bearing temperature sensor | Temp > 85 °C | Alarms at 75 °C; Trips at 85 °C | Each bearing housing |
| Feed chute plug detector | Rotation sensor < 2 rpm | Stops feed screw; alarms | Feed hopper screw |
| Cryogenic mill — O₂ sensor | O₂ > 1.5 % vol in exhaust | Stops mill; vents N₂; alarms | Exhaust duct |
| Cryogenic mill — low N₂ pressure | N₂ pressure < 0.3 MPa | Stops feed; maintains N₂ purge | N₂ supply line |
| Cryogenic mill — door seal pressure | Seal pressure < 0.1 MPa | Does not start / stops mill | Chamber door |
| Metal detector reject confirmation | Reject signal not confirmed in 2 s | Stops belt / conveyor downstream | Metal detector exit |

---

## 9. Utility Requirements

| Utility | Specification | Connection | Consumption (per line) |
|---------|---------------|------------|------------------------|
| Electrical power | 380–480 V, 3-phase, 50/60 Hz | Hardwired to MCC | 55 kW (peak, hammer mill); 80 kW (cryogenic) |
| Compressed air | 0.6–0.8 MPa, oil-free, dry (dew point −20 °C) | 3/4″ NPT | 0.8 m³/min (pneumatic gates, metal ejector) |
| Liquid nitrogen (cryogenic mill) | −196 °C, 99.99 % purity, 0.8 MPa max | Vacuum-jacketed pipe, DN25 | 1,000 kg/MT product |
| Cooling water (cryogenic heat exchanger) | 10–20 °C, 0.3 MPa, SS304 line | 2″ flange | 30 L/min |
| Dust extraction | 100 m³/min at −3 kPa | 200 mm duct flange | 15 kW fan |
| Plant air ventilation (O₂ monitoring area) | 6 air changes/hr | — | 5 kW fan |

---

## 10. Common Spare Parts List

| Part | Part Number (Example) | Qty in Stock | Lead Time | Criticality |
|------|-----------------------|--------------|-----------|-------------|
| Hammer set — AR400 (24 pcs) | SB‑HAM‑24‑AR400 | 2 sets | 1 week | High |
| Screen basket — 1.5 mm (SS304) | SB‑SCR‑15‑304 | 2 | 2 weeks | High |
| Screen basket — 3.0 mm (SS304) | SB‑SCR‑30‑304 | 1 | 2 weeks | Medium |
| Screen basket — 0.8 mm (SS304) | SB‑SCR‑08‑304 | 2 | 2 weeks | High |
| Disc mill disc pair (Ni-hard) | MJZS‑80‑DISC‑PAIR | 1 | 8 weeks | High |
| Pin mill rotor pin disc (complete) | 160UPZ‑ROT‑DISC | 1 | 10 weeks | High |
| Pin mill stator pin disc (complete) | 160UPZ‑STAT‑DISC | 1 | 10 weeks | High |
| Pin mill pin — WC-Co (single) | 160UPZ‑PIN‑WC | 100 | 1 week | Medium |
| Cryogenic mill — shaft seal kit | CG‑SEAL‑KIT | 2 | 4 weeks | High |
| Cryogenic mill — PTFE door gasket | CG‑GASK‑DOOR | 4 | 2 weeks | High |
| Cryogenic mill — N₂ injection nozzle | CG‑NOZ‑LN2 | 3 | 6 weeks | Medium |
| Metal detector test wand set (Fe/SS/Cu) | Safeline‑TEST‑SET | 2 | 1 week | High |
| Mill motor — bearing set (SKF 6317 / 7317) | SKF‑6317‑C3 | 4 each | 1 week | Medium |
| VFD — spare drive (55 kW) | Siemens G120 / ABB ACS880 | 1 | 4 weeks | High |
| Food-grade grease — Klüber 4-302 | — | 5 kg | 2 weeks | Low |

---

## 11. Calibration Requirements

| Instrument / Device | Range | Standard | Tolerance | Calibration Frequency | Responsibility |
|---------------------|-------|----------|-----------|-----------------------|----------------|
| Mill tachometer (all mills) | 0–15,000 rpm | Stroboscope | ±10 rpm | 6 months | Maintenance |
| Feeler gauge (screen clearance / disc gap) | 0.05–2.00 mm | Micrometer (NIST-traceable) | ±0.01 mm | 6 months | QC |
| Sieve shaker (particle size QC) | 38 µm–4.75 mm | ASTM E11 calibration sieves | ±2 % aperture | 12 months | QC lab |
| Laser diffraction analyser (cryogenic QC) | 0.01–2,000 µm | NIST SRM 114P | ±3 % d50 | 12 months | QC / external lab |
| Cryogenic mill — Pt100 RTD | −200 to +50 °C | Ice-point + dry-well calibrator | ±0.5 °C | 6 months | QC |
| Cryogenic mill — O₂ analyser | 0–25 % vol | Certified calibration gas (1 % O₂ in N₂) | ±0.1 % | 3 months | QC / external |
| Cryogenic mill — N₂ flow meter | 0–5 kg/min | Coriolis master meter | ±0.5 % of reading | 12 months | Maintenance |
| Metal detector (CCP-2) | Fe ≥ 1.0 mm, SS ≥ 1.5 mm, Cu ≥ 1.5 mm | Certified test wands (traceable to NIST) | 100 % detection at critical limit | Start of each shift (function); 6 months (full cal) | Operator (daily); OEM (annual) |
| Energy meter (kWh) | 0–100 kW | Reference power analyser | ±0.5 % | 12 months | Electrical tech |
| IR thermometer (product temp) | 0–100 °C | Blackbody calibrator | ±1 °C | 6 months | QC |

---

*Document version: 1.0 — Author: Process Engineering — Approved: QA Manager*
