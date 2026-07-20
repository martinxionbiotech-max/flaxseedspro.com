# Dehulling & Separation Equipment — Technical Specification

## 1. Process Objective

Remove the fibrous hull from pre-conditioned flaxseed while minimising endosperm breakage, then classify the stream into hulls, coarse middlings, and clean kernels. Design capacity: **3 MT/hr** input. Target dehulling efficiency: **85–90 %**.

---

## 2. Equipment Configuration — ASCII Flow Diagram

```
Pre-conditioned flaxseed (3 MT/hr, from tempering)
      |
      v
[ 1. Centrifugal Impact Dehuller ]         ← 3,000–4,500 rpm   Primary break
      |   (impeller + stator ring)
      |
      v
[ 2. Roller Dehuller ]                      ← 0.3–0.8 mm gap   Secondary break
      |
      v
[ 3. Air Classifier — Zigzag Column ]       ← Hull removal (light fraction)
      |
      v
[ 4. Gravity Separator — Deck table ]       ← Kernel / mid-density separation
      |
      v
      +──→ Hull fraction (to pelletising / waste)
      +──→ Middlings (to grinding)
      +──→ Clean kernels (to packaging / further processing)
```

---

## 3. Equipment Table

| Unit | Type | Model (Example) | Capacity (MT/hr) | Power (kW) | Material (food-contact) | Manufacturer (suggested) |
|------|------|-----------------|-------------------|------------|------------------------|--------------------------|
| Centrifugal Impact Dehuller | Vertical impeller with tungsten-carbide pins & stator ring | Retsch ZM-500 / custom | 3–4 | 22–30 | SS304 chamber, WC-Co pins, SS304 stator | Hosokawa / Retsch / custom |
| Roller Dehuller | Twin paired rolls, differential speed | Bühler MDDL-800 | 3–5 | 2 × 7.5 | Chilled cast-iron rolls, SS304 frame | Bühler / Satake |
| Air Classifier (Zigzag) | Zigzag column + fan + cyclone | Rhewum ZAZ-600 | 3–6 | 11 (fan) + 1.5 (feeder) | SS304 column & cyclone | Rhewum / Hosokawa Alpine |
| Gravity Separator | Reciprocating deck, air-table | Forsberg GC-48 | 3–4 | 5.5 (fan) + 1.5 (drive) | SS304 expanded-metal deck, polycarbonate cover | Forsberg / Oliver |

---

## 4. Detailed Technical Parameters — Set Points & Tolerances

### 4.1 Centrifugal Impact Dehuller (3,000–4,500 rpm)

| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Impeller rotational speed | 3,600 rpm | ±100 rpm | VFD-controlled |
| Tip speed (impeller outer Ø 400 mm) | 75 m/s | ±5 m/s | Critical for hull release |
| Number of impact pins (impeller) | 12 | — | Replaceable tungsten-carbide |
| Number of impact pins (stator ring) | 24 | — | Tungsten-carbide coated |
| Pin-to-pin gap (stator vs. impeller) | 8 mm | ±0.5 mm | Adjustable via shims |
| Feed rate per rotor | 3 MT/hr | ±0.3 MT/hr | — |
| Product temperature at inlet | 35–50 °C | ±5 °C | From tempering |
| Dehulling efficiency (target) | 85 % | ±3 % | Sieve + visual count |
| Broken kernel / fines generation | ≤ 5 % | — | Target < 2 % for premium |
| Amperage (no-load) | 15 A | ±2 A | At 380 V, 50 Hz |

### 4.2 Roller Dehuller

| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Roll diameter | 250 mm | ±0.5 mm | Chilled cast iron |
| Roll length | 800 mm | ±1 mm | — |
| Fast roll speed | 800 rpm | ±10 rpm | — |
| Slow roll speed | 450 rpm | ±10 rpm | Ratio ~1.78:1 |
| Roll gap (nip) — fixed side | 0.5 mm | ±0.05 mm | Adjustable by eccentric |
| Roll gap — floating side | 0.5 mm | ±0.05 mm | Spring-loaded |
| Differential speed ratio | 1.78 : 1 | ±0.05 | — |
| Feed rate | 3 MT/hr | ±0.3 MT/hr | Even curtain across roll width |
| Motor load (each roll) | ≤ 7.5 kW | — | Thermal overload relay |
| Roll surface hardness | 58–62 HRC | ±2 HRC | — |

### 4.3 Air Classifier — Zigzag Column

| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Air velocity in column | 6.0 m/s | ±0.5 m/s | Adjustable damper / VFD fan |
| Column height | 2,000 mm | ±50 mm | 8 zigzag stages |
| Zigzag angle | 45° | ±2° | — |
| Cut point (d50) | 1.2 mm | ±0.1 mm | Hulls < 1.2 mm rise |
| Feed rate | 3 MT/hr | ±0.3 MT/hr | — |
| Fan volume | 120–150 m³/min | ±10 m³/min | — |
| Static pressure at fan inlet | −1.5 kPa | ±0.2 kPa | — |
| Hull recovery (light fraction) | ≥ 90 % | — | Hull purity ≥ 85 % |
| Kernel loss to hull fraction | ≤ 5 % | — | Target < 3 % |

### 4.4 Gravity Separator (Deck Table)

| Parameter | Set Point | Tolerance | Notes |
|-----------|-----------|-----------|-------|
| Deck air velocity | 3.0–4.5 m/s | ±0.3 m/s | Adjustable plenum |
| Deck vibration frequency | 600–800 rpm | ±10 rpm | — |
| Deck longitudinal incline | 5°–8° | ±0.5° | Product travel |
| Deck transverse incline | 2°–4° | ±0.5° | Side discharge separation |
| Feed rate | 3 MT/hr | ±0.3 MT/hr | — |
| Kernel purity (heavy fraction) | ≥ 98 % | — | — |
| Hull purity (light fraction) | ≥ 85 % | — | — |
| Full separation efficiency | ≥ 90 % | — | Composite of all fractions |

---

## 5. Performance Targets & Verification

| Parameter | Target | Verification Method | Frequency |
|-----------|--------|---------------------|-----------|
| Dehulling efficiency (overall) | 85–90 % | Sieve fractionation + manual hull count | Every 2 hr |
| Broken / damaged kernels | ≤ 5 % | Visual + sieve (0.5 mm pan) | Every 2 hr |
| Hull removal rate (air classifier) | ≥ 90 % | Weight of light fraction vs. calculated hull content | Daily |
| Kernel purity after gravity separator | ≥ 98 % | Hand-pick separation of 500 g sample | Daily |
| Throughput | 3 MT/hr ± 0.3 | Belt scale / weigh hopper | Continuous |
| Power consumption per ton | ≤ 15 kWh/MT | Energy meter | Monthly |

---

## 6. HACCP Integration

NOTE: Dehulling stages do not constitute a CCP under standard flaxseed HACCP plans (hazards are physical/quality, not critical food safety). They are **OPRPs (Operational Prerequisite Programs)**.

### OPRP-1 — Centrifugal Impact Dehuller & Roller Dehuller

| Element | Specification |
|---------|--------------|
| **Hazard** | Physical — metal fragments from pin/roll wear; Excessive fines generation |
| **Control Measure** | Regular pin/roll gap inspection; metal detector downstream (CCP-2 in grinding area) |
| **Monitoring** | Operator checks pin wear (visual) & roll gap (feeler gauge) |
| **Frequency** | Every 4 hr |
| **Corrective Action** | Replace worn pins; re-set roll gap; divert product until verified |
| **Record** | OPRP log sheet |

### OPRP-2 — Air Classifier & Gravity Separator

| Element | Specification |
|---------|--------------|
| **Hazard** | Cross-contamination — improper separation leaving hull fragments in kernels |
| **Control Measure** | Air velocity & deck incline set points; periodic analysis of outlet streams |
| **Monitoring** | QC analyses of hull & kernel streams |
| **Frequency** | Every 4 hr |
| **Corrective Action** | Re-adjust air velocity / incline; re-screen material |
| **Record** | OPRP log sheet |

---

## 7. Maintenance Schedule

### 7.1 Daily (shift-end, ~25 min total)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Centrifugal impact dehuller — check pin wear (visual); clear any wrap-around | 5 | Operator |
| Roller dehuller — check roll gap with feeler gauge; wipe rolls clean | 5 | Operator |
| Air classifier — empty cyclone bag; check air velocity manometer | 5 | Operator |
| Gravity separator — clean deck surface; check air plenum for blockage | 5 | Operator |
| Log all readings in CMMS | 5 | Operator |

### 7.2 Weekly (~2.5 hr)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Centrifugal dehuller — remove impeller; measure pin tip diameter; replace if worn < 80 % original | 30 | Maintenance tech |
| Roller dehuller — check roll surface flatness (dial gauge); re-set eccentric if runout > 0.05 mm | 30 | Maintenance tech |
| Air classifier — clean zigzag stages; inspect for wear | 30 | Operator |
| Gravity separator — deck fabric / expanded-metal inspection | 15 | Maintenance tech |
| Lubricate feed screw gearboxes (food-grade oil) | 15 | Maintenance tech |
| All belts & chains — tension check | 15 | Maintenance tech |
| VFD parameters & motor current logging | 15 | Electrical tech |

### 7.3 Monthly (~5 hr)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Centrifugal dehuller — replace all stator pins; rotate impeller if applicable | 60 | Maintenance tech |
| Roller dehuller — remove rolls; measure OD for re-grinding / replacement (min. Ø 245 mm) | 60 | Maintenance tech |
| Air classifier — fan impeller balance check; bearing re-grease | 30 | Maintenance tech |
| Gravity separator — deck replacement if worn; plenum seal inspection | 60 | Maintenance tech |
| All bearings replacement (as needed based on vibration data) | 30 | Maintenance tech |
| Clean all dust collection lines & cyclones | 30 | Operator |
| Update spare parts inventory | 30 | Maintenance lead |

### 7.4 Annual (during shutdown, ~16 hr)

| Task | Time (min) | Performed By |
|------|------------|--------------|
| Centrifugal dehuller — replace entire impeller & stator ring assembly | 120 | Maintenance team |
| Roller dehuller — re-grind or replace rolls; replace all bearings & seals | 240 | Maintenance team |
| Air classifier — complete fan replacement (impeller + shaft + bearings) | 120 | Maintenance tech |
| Gravity separator — rebuild drive mechanism (eccentric, springs, bushings) | 180 | Maintenance team |
| All motors — Megger test (insulation > 20 MΩ) + re-grease | 120 | Electrical tech |
| All — structural inspection; weld repair; repaint food-contact surfaces | 120 | Maintenance team |
| Full HACCP / OPRP validation — run 8-hr qualification batch | 240 | QC + Production |

---

## 8. Safety Interlocks & Emergency Stops

| Interlock / E-Stop | Trigger | Action | Location |
|--------------------|---------|--------|----------|
| E-Stop pushbutton (red mushroom) | Manual press | Isolates all drive motors; brake on conveyors | Each equipment panel + line ends |
| Centrifugal dehuller door interlock | Access door sensor | Stops impeller if door opened | Dehuller chamber door |
| Roller dehuller nip guard | Magnetic switch on roll cover | Stops rolls; disengages clutch | Roll cover panel |
| Air classifier fan overtemp | PTC thermistor (set 140 °C) | Trips fan VFD | Fan motor winding |
| Gravity separator vibration sensor | Excessive vibration > 8 mm/s | Stops deck drive | Drive housing |
| Feed chute plug detector | Rotation sensor on feed screw | Stops upstream feed | Each chute |
| Compressed air low pressure | Pressure switch < 0.4 MPa | Stops all pneumatic systems | Air manifold |

---

## 9. Utility Requirements

| Utility | Specification | Connection | Consumption (per line) |
|---------|---------------|------------|------------------------|
| Electrical power | 380–480 V, 3-phase, 50/60 Hz | Hardwired to MCC | 45 kW (peak) |
| Compressed air | 0.6–0.8 MPa, oil-free, dry (dew point −20 °C) | 1″ NPT | 1.2 m³/min (pneumatic gates only) |
| Dust collection | 150 m³/min at −3 kPa | 250 mm duct flange | 11 kW fan |
| Lighting | 500 lux minimum at deck level | Ceiling-mounted LED | 0.3 kW |

---

## 10. Common Spare Parts List

| Part | Part Number (Example) | Qty in Stock | Lead Time | Criticality |
|------|-----------------------|--------------|-----------|-------------|
| Impeller pins (WC-Co) — set of 12 | CID‑PIN‑WC‑12 | 3 sets | 2 weeks | High |
| Stator pins (WC-Co) — set of 24 | CID‑STAT‑WC‑24 | 2 sets | 2 weeks | High |
| Impeller assembly (complete) | CID‑IMP‑400‑SS | 1 | 8 weeks | High |
| Roller pair (matched, chilled cast iron Ø250×800) | RD‑250‑800‑PAIR | 1 | 12 weeks | High |
| Roller bearings — SKF 22218 E | SKF‑22218‑E | 4 | 1 week | Medium |
| Zigzag column panel (SS304) | ZAZ‑PAN‑2000 | 2 | 4 weeks | Low |
| Gravity separator deck (expanded metal) | GC‑48‑DECK | 1 | 6 weeks | Medium |
| Gravity separator eccentric bushing | GC‑ECC‑BUSH | 2 | 3 weeks | Medium |
| Fan impeller (air classifier) | ZAZ‑FAN‑IMP‑630 | 1 | 8 weeks | Low |
| Food-grade grease — Klüber 4-302 | — | 5 kg | 2 weeks | Low |
| V-belt set — SPB-2240 | Gates / Optibelt | 6 | 1 week | Medium |
| Manometer diaphragm (0–2 kPa) | — | 2 | 2 days | Low |

---

## 11. Calibration Requirements

| Instrument / Device | Range | Standard | Tolerance | Calibration Frequency | Responsibility |
|---------------------|-------|----------|-----------|-----------------------|----------------|
| Hand tachometer (dehuller rpm) | 0–9,999 rpm | Stroboscope | ±5 rpm | 12 months | Maintenance |
| Feeler gauge set (roll gap) | 0.05–1.00 mm | Micrometer (NIST-traceable) | ±0.01 mm | 6 months | QC |
| Anemometer (air classifier) | 0–15 m/s | NIST-traceable Pitot tube | ±0.2 m/s | 12 months | Maintenance |
| Pressure manometer (gravity sep.) | 0–2 kPa | Water-column manometer | ±20 Pa | 6 months | QC |
| VFD speed display | 0–60 Hz | Oscilloscope + frequency counter | ±0.1 Hz | 12 months | Electrical tech |
| Belt scale (throughput) | 0–5 MT/hr | Test weights (50 kg certified) | ±0.5 % | 6 months | Maintenance |
| Temperature probe (product inlet) | 0–100 °C | NIST-traceable Pt100 | ±0.5 °C | 12 months | QC |

---

*Document version: 1.0 — Author: Process Engineering — Approved: QA Manager*
