# Cleaning & Grading Equipment — Technical Specification

## 1. Process Objective

Remove foreign matter (ferrous/non-ferrous metals, stones, fines, off-color seeds) from raw flaxseed at a design capacity of **8 MT/hr**. Four-stage dry cleaning: magnetic separation → vibratory screening → aspiration → destoning → color sorting.

---

## 2. Equipment Configuration — ASCII Flow Diagram

```
raw flaxseed (8 MT/hr)
      |
      v
[ Hopper / Elevator ]
      |
      v
[ 1. Magnet — 10,000 Gauss ]               ← Ferrous removal
      |
      v
[ 2. Vibrating Screen — 4 decks ]          ← Overs/sizing
      |  4 mm / 2 mm / 1 mm / 0.5 mm
      v
[ 3. Aspirator — 4–6 m/s air ]            ← Light fines / hulls
      |
      v
[ 4. Destoner — Fluidized bed ]            ← Stones / heavy contaminants
      |
      v
[ 5. Color Sorter — NIR+VIS, 128 ch. ]    ← Discolored / defective seeds  (CCP-1)
      |
      v
[ Clean flaxseed to tempering silo ]
```

---

## 3. Equipment Table

| Unit | Type | Model (Example) | Capacity (MT/hr) | Power (kW) | Material (food-contact) | Manufacturer (suggested) |
|------|------|-----------------|-------------------|------------|------------------------|--------------------------|
| Permanent Magnet | Drawer / Cartridge, 10,000 Gauss | Eriez SE-7830 | 8–10 | — | SS304 housing, magnets Ni-plated NdFeB | Eriez / Bunting |
| Vibrating Screen | Gyratory / Linear, 4-deck | Sweco 84" X-Screen | 8–10 | 2 × 2.2 (vibrators) | SS304 / 316L screen frames, food-grade silicone balls | Sweco / Kason |
| Aspirator | Vertical air column + cyclone | Forsberg 2S-48 | 8–12 | 7.5 (fan) + 0.75 (feeder) | SS304 contact surfaces | Forsberg / Oliver |
| Destoner | Fluidized-bed / air-table | Oliver MCS-48 | 8–10 | 5.5 (fan) + 0.75 (drive) | SS304 deck, polycarbonate cover | Oliver / Sortex |
| Color Sorter | NIR + VIS belt-type, 128 ch. | Satake SC-2000Z | 6–10 | 2.5 + 1.5 (compressor) | Food-grade conveyor, SS304 frame | Satake / Bühler / Tomra |

---

## 4. Detailed Technical Parameters — Set Points & Tolerances

### 4.1 Magnet (10,000 Gauss)
| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Magnetic field strength | 10,000 G | ±500 G | At pole face |
| Material temperature | 25 °C | −10 / +40 °C | Above 60 °C demagnetises |
| Drawer pull-out force | > 15 kgf | — | Manual cleaning threshold |

### 4.2 Vibrating Screen (4-deck)
| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Deck 1 (overs) | 4.0 mm | ±0.1 mm | Round / square perforation |
| Deck 2 (middlings) | 2.0 mm | ±0.1 mm | — |
| Deck 3 (fines) | 1.0 mm | ±0.05 mm | — |
| Deck 4 (ultra-fines) | 0.5 mm | ±0.05 mm | — |
| Vibration frequency | 960–1,440 rpm | ±20 rpm | Adjustable eccentric |
| Stroke (throw) | 6–12 mm | ±1 mm | — |
| Deck incline | 5°–8° | ±0.5° | — |
| Feed rate | 8 MT/hr | ±0.5 MT/hr | — |

### 4.3 Aspirator (4–6 m/s)
| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Air velocity in column | 5.0 m/s | ±0.5 m/s | Adjustable damper |
| Air volume | 60–80 m³/min | ±5 m³/min | — |
| Feed gate opening | 70 % | ±5 % | — |
| Cyclone pressure drop | 800–1,200 Pa | ±100 Pa | — |
| Light fraction removal | ≥ 98 % | — | Verify by sieve analysis |

### 4.4 Destoner (Fluidized Bed)
| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Deck air velocity | 3.5–5.0 m/s | ±0.3 m/s | Adjustable plenum |
| Deck vibration | 500–700 rpm | ±10 rpm | — |
| Deck incline (long.) | 4°–8° | ±0.5° | — |
| Deck incline (trans.) | 2°–5° | ±0.5° | — |
| Plenum pressure | 600–900 Pa | ±50 Pa | — |
| Stone removal efficiency | ≥ 99.5 % | — | — |

### 4.5 Color Sorter (NIR+VIS, 128 ch.) — CCP-1
| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Number of channels | 128 | — | 64 NIR + 64 VIS |
| NIR wavelength range | 950–1,700 nm | ±10 nm | Indium Gallium Arsenide |
| VIS wavelength range | 400–1,050 nm | ±10 nm | Silicon CCD |
| Reject sensitivity | User-adjustable | 0–999 | Digital threshold |
| Ejector air pressure | 0.5–0.7 MPa | ±0.05 MPa | Compressed air |
| Ejector firing duration | 5–15 ms | ±1 ms | Per channel |
| Feed rate (per chute) | 60–80 kg/hr | ±10 kg/hr | — |
| Belts speed | 2.0–4.0 m/s | ±0.2 m/s | — |
| Reject ratio (target) | ≤ 3 % | — | Of total good product |

---

## 5. Performance Targets & Verification

| Parameter | Target | Verification Method | Frequency |
|-----------|--------|---------------------|-----------|
| Ferrous removal | ≥ 99.9 % | Magnet check / ferrous test piece | Daily |
| Overs separation | ≤ 0.5 % fines in overs | Sieve analysis (Ro-Tap) | Weekly |
| Aspirator light fraction removal | ≥ 98 % | Sieve + weight check | Weekly |
| Destoner stone removal | ≥ 99.5 % | Stone spiking test | Monthly |
| Color sorter reject accuracy | ≥ 99.5 % defect removal | Calibrated plastic seeds / sample | Daily shift start |
| Total throughput | 8 MT/hr ± 0.5 | Belt scale / weigh hopper | Continuous |
| Power consumption | ≤ 22 kW (all units) | Energy meter logging | Monthly |

---

## 6. HACCP Integration — CCP-1 (Color Sorter)

| Element | Specification |
|---------|--------------|
| **CCP ID** | CCP-1 |
| **Hazard** | Physical (foreign material) + Organoleptic (discoloured/mouldy seeds → mycotoxin risk) |
| **Critical Limit** | ≤ 0.02 % discoloured/foreign seeds in outgoing product (by weight) |
| **Monitoring Device** | NIR+VIS camera array + pneumatic ejectors; PLC logs reject count per minute |
| **Monitoring Frequency** | Continuous during production; manual check with sample tray every 30 min |
| **Monitoring Personnel** | Line operator |
| **Corrective Action** | 1. Pause production at CCP-1. 2. Divert in-process material. 3. Re-calibrate sensitivity. 4. Log incident. |
| **Verification** | Lab colour-sort audit every 4 hr; third-party check weekly |
| **Record Keeping** | CCP log sheet (hourly); digital PLC archive (30-day retention) |

### Supporting HACCP for Pre-Cleaning Stages

| Equipment | Hazard Controlled | Monitoring | Frequency |
|-----------|-------------------|------------|-----------|
| Magnet (10k Gauss) | Ferrous metal | Visual check + ferrous test piece | Every shift |
| Vibrating screen | Oversize debris / lumps | Screen deck integrity inspection | Daily |
| Aspirator | Dust / light chaff | Air velocity manometer check | Daily |
| Destoner | Stones / heavy metals | Stone collection tray inspection | Daily |

---

## 7. Maintenance Schedule

### 7.1 Daily (shift-end, ~30 min total)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Magnet — remove & clean accumulated ferrous material | 5 | Operator |
| Vibrating screen — visual check for torn/blocked screens | 5 | Operator |
| Aspirator — empty cyclone collection bag; check air velocity | 5 | Operator |
| Destoner — empty stone collection tray; check fluidisation | 5 | Operator |
| Color sorter — clean camera lenses & windows (lint-free cloth) | 5 | Operator |
| All — log readings in CMMS | 5 | Operator |

### 7.2 Weekly (~2 hr)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Screen deck change-out inspection (swap with spare if > 5 % blinding) | 30 | Maintenance tech |
| Magnet Gauss measurement (handheld Gaussmeter) — re-charge if < 9,500 G | 15 | QC / Tech |
| Aspirator fan belt tension & pulley alignment check | 15 | Maintenance tech |
| Destoner air plenum filter cleaning | 15 | Operator |
| Color sorter nozzle bank check — fire test pattern | 30 | Maintenance tech |
| All threaded fasteners torque check | 15 | Maintenance tech |

### 7.3 Monthly (~4 hr)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Complete magnet assembly removal & degaussing check | 30 | Maintenance tech |
| Vibrating screen — replace worn screen cloth as needed | 60 | Maintenance tech |
| Aspirator — cyclone & ducting inspection for wear | 30 | Maintenance tech |
| Destoner — deck surface wear measurement; replace if < 3 mm | 30 | Maintenance tech |
| Color sorter — full calibration with reference sample set | 60 | QC + Tech |
| Lubricate all bearings (food-grade grease) | 30 | Maintenance tech |
| Update maintenance log & spare parts inventory | 30 | Maintenance lead |

### 7.4 Annual (during shutdown, ~16 hr)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Magnet — factory recertification of Gauss rating | — | OEM / external lab |
| Vibrating screen — full frame re-level; replace all springs & balls | 240 | Maintenance team |
| Aspirator — fan impeller balancing & bearing replacement | 120 | Maintenance tech |
| Destoner — complete deck removal, re-surfacing or replacement | 180 | Maintenance team |
| Color sorter — full optical bench alignment + lamp replacement | 180 | OEM service engineer |
| All motors — insulation resistance test (Megger) & re-grease | 120 | Electrical tech |
| All — structural integrity check, weld inspection, electric panel clean | 120 | Maintenance team |

---

## 8. Safety Interlocks & Emergency Stops

| Interlock / E-Stop | Trigger | Action | Location |
|--------------------|---------|--------|----------|
| Emergency stop (red pushbutton) | Manual press | Isolates all motors & air; brake on belt conveyors | Each equipment panel + central |
| Magnet door interlock | Access door opened | Cuts feed conveyor upstream | Magnet housing |
| Screen access door | Vibration sensor on guard | Stops vibrator motors if guard lifted | Screen frame |
| Aspirator fan overtemp | Thermal overload relay (set 140 °C) | Trips fan motor | Fan motor starter |
| Destoner air pressure low | Pressure switch < 300 Pa | Stops feed roller | Destoner plenum |
| Color sorter enclosure | Interlock on camera housing | Disables ejector air; keeps belts running | Camera enclosure |
| Overall line E-Stop pull-cord | Pulled at any point | Full line stop in < 2 s | Along conveyor length |

---

## 9. Utility Requirements

| Utility | Specification | Connection | Consumption (per line) |
|---------|---------------|------------|------------------------|
| Electrical power | 380–480 V, 3-phase, 50/60 Hz | Hardwired to MCC | 22 kW (peak) |
| Compressed air | 0.6–0.8 MPa, oil-free, dry (dew point −20 °C) | 1″ NPT quick-connect | 2.5 m³/min (color sorter) |
| Lighting (inspection) | 1,000 lux at camera plane | Dedicated LED | 0.5 kW |
| Exhaust / dust collection | 80 m³/min at −2 kPa | 200 mm duct flange | 7.5 kW fan |

---

## 10. Common Spare Parts List

| Part | Part Number (Example) | Qty in Stock | Lead Time | Criticality |
|------|-----------------------|--------------|-----------|-------------|
| Magnet cartridge assembly (10k G) | Eriez P-TRAP-7830 | 1 | 4 weeks | High |
| Screen cloth — 4 mm SS | Sweco 84‑4.0‑304 | 2 rolls | 2 weeks | Medium |
| Screen cloth — 2 mm SS | Sweco 84‑2.0‑304 | 2 rolls | 2 weeks | Medium |
| Screen cloth — 1 mm SS | Sweco 84‑1.0‑304 | 2 rolls | 2 weeks | Medium |
| Screen cloth — 0.5 mm SS | Sweco 84‑0.5‑304 | 2 rolls | 2 weeks | Medium |
| Silicone ball deck cleaners | Sweco 38 mm silicone | 500 | 1 week | Medium |
| Aspirator fan belt — SPZ-1900 | Gates / Optibelt | 4 | 1 week | Low |
| Destoner deck fabric | Oliver MCS-48 deck | 1 | 6 weeks | High |
| Color sorter LED lamp (VIS) | Satake HL‑VIS‑128 | 2 | 8 weeks | High |
| Color sorter NIR lamp | Satake HL‑NIR‑128 | 1 | 8 weeks | High |
| Ejector valve (solenoid + nozzle) | Satake EV‑128‑12 | 4 | 4 weeks | High |
| Air filter regulator (FRL) | SMC AW40‑F04 | 2 | 1 week | Low |
| Food-grade grease | Klüber Lubricant 4‑302 | 5 kg | 2 weeks | Low |

---

## 11. Calibration Requirements

| Instrument / Device | Range | Standard | Tolerance | Calibration Frequency | Responsibility |
|---------------------|-------|----------|-----------|-----------------------|----------------|
| Handheld Gaussmeter | 0–20,000 G | NIST-traceable reference magnet | ±100 G | 6 months | QC / external lab |
| Digital tachometer (screen rpm) | 0–9,999 rpm | Stroboscope | ±5 rpm | 12 months | Maintenance |
| Anemometer / hot-wire (aspirator) | 0–20 m/s | NIST-traceable Pitot tube | ±0.1 m/s | 12 months | Maintenance |
| Pressure manometer (destoner) | 0–2,000 Pa | Water-column manometer | ±10 Pa | 6 months | QC |
| Color sorter reference sample set | Colour tiles (white, black, red, green) | Spectrophotometer (Lab values) | ΔE < 0.5 | 1 month (new set every 6 months) | QC lab |
| Belt scale (throughput) | 0–15 MT/hr | Test weights (50 kg certified) | ±0.5 % | 6 months | Maintenance |
| PLC process timer | 0–10 s | Oscilloscope / stopwatch | ±10 ms | 12 months | Electrical tech |

---

*Document version: 1.0 — Author: Process Engineering — Approved: QA Manager*
