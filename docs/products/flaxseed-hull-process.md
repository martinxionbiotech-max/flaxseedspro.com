# Flaxseed Hull Processing — Process & Workflow Document

> **Document ID:** PROD-HULL-001  
> **Version:** 1.0  
> **Last Updated:** 2026-07-20  
> **Product:** Flaxseed Hull Powder (FHP)

---

## 1. Process Overview

The flaxseed hull process extracts the outer fibrous hull layer from cleaned flaxseed, producing a concentrated lignan- and fiber-rich hull powder. The process is designed to maximize hull yield while minimizing kernel contamination and preserving bioactive compound integrity.

### 1.1 Process Flow Summary

```
Cleaned Seed → Conditioning → Dehulling → Air Classification
    → Hull Stream → Milling → Sifting → Hull Powder → Packaging
```

### 1.2 High-Level Parameters

| Parameter | Target | Tolerance |
|-----------|--------|-----------|
| Overall yield (hull basis) | 22–28% | ±2% |
| Hull purity (lignan content) | ≥ 2.5% SDG | ±0.3% |
| Moisture (final product) | ≤ 6.0% | ±0.5% |
| Particle size (D90) | ≤ 250 µm | ±20 µm |

---

## 2. Detailed Process Stages

### 2.1 Cleaned Seed (Input)

**Purpose:** Receive and hold flaxseed that has passed through CCP-1 (Cleaning — Metal Detection & Sieving).

**Equipment:**
- Stainless steel receiving hopper (2,000 kg capacity)
- Bucket elevator with magnetic head pulley
- Surge bin with level sensors (5,000 kg)
- Screw conveyor

**Parameters:**
- Receiving temperature: Ambient (15–30°C)
- Holding time: ≤ 48 hours prior to conditioning
- Moisture at receiving: 6.0–9.5%
- Foreign material: ≤ 0.5% (validated per incoming QC)

**Quality Check: Incoming Verification**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Moisture | Per lot | NIR / Oven drying | 6.0–9.5% | > 10% → reject lot |
| Foreign matter | Per lot | Sieve analysis + visual | ≤ 0.5% | > 1.0% → re-clean or reject |
| Oil content | Per supplier lot | NMR | 38–44% | Out of spec → supplier notification |
| SDG lignan content | Monthly composite | HPLC | ≥ 1.2% dry basis | < 1.0% → reformulate blend |

---

### 2.2 Conditioning

**Purpose:** Heat and moisturize seeds to loosen the hull-kernel bond for efficient dehulling.

**Equipment:**
- Vertical stack conditioner (3-tray, steam-jacketed)
- Tempering bin (jacketed, variable-speed discharge)
- Steam generator (low-pressure, 2–3 bar)

**Parameters:**

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Conditioning temperature | 65°C | 60–70°C | Steam valve PID |
| Seed moisture after conditioning | 10.0% | 9.5–10.5% | Water spray nozzles |
| Conditioning time | 20 min | 15–25 min | Conveyor speed |
| Steam pressure | 2.5 bar | 2.0–3.0 bar | Regulator |
| Bed depth | 15 cm | 12–18 cm | Gate position |

**Process Notes:**
- Over-conditioning (>70°C or >25 min) causes hull sticking and oil migration
- Under-conditioning (<55°C) results in excessive kernel breakage
- Steam must be culinary-grade (filtered, no boiler additives)

**Quality Check: Conditioning Effectiveness**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Seed temp. after conditioning | Every 30 min | IR probe | 60–70°C | > 72°C → reduce steam |
| Moisture | Every batch | NIR | 9.5–10.5% | < 9.0% → increase spray; > 11% → hold & adjust |
| Hull detachment test | Every 2 hours | Hand-squeeze test (50 seeds) | ≥ 80% detach | < 70% → increase conditioning time/temp |

---

### 2.3 Dehulling

**Purpose:** Mechanically fracture and separate the hull from the kernel using impact and shear forces.

**Equipment:**
- Centrifugal dehuller (impact disc, 3,000–4,500 rpm)
- Gap-adjustable roller dehuller (corrugated rolls, differential speed)
- Aspiration pre-separator

**Parameters:**

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Impact disc speed | 3,800 rpm | 3,500–4,200 rpm | VFD |
| Roll gap (roller dehuller) | 0.8 mm | 0.6–1.0 mm | Manual micrometer adjust |
| Differential roll speed | 1.5:1 | 1.3:1–1.7:1 | Gear ratio |
| Feed rate | 800 kg/h | 600–1,000 kg/h | Screw feeder VFD |
| Aspiration air velocity | 5 m/s | 4–6 m/s | Damper control |

**Process Notes:**
- Higher RPM increases hull yield but also fines generation
- Roll gap < 0.5 mm causes kernel damage; > 1.5 mm leaves hulls intact
- Monitor amperage on impact disc motor — spike indicates plugging risk

**Quality Check: Dehulling Efficiency**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Dehulling efficiency | Every hour | Sieve analysis (2 mm screen) | ≥ 85% hull release | < 80% → adjust RPM/gap |
| Whole kernel breakage | Every hour | Hand sorting (100 g sample) | ≤ 5% broken | > 8% → reduce RPM |
| Fines (< 500 µm) | Every 2 hours | Sieve analysis | ≤ 12% | > 15% → adjust aspiration |

---

### 2.4 Air Classification

**Purpose:** Separate the lighter hull fraction from heavier kernel pieces using controlled air streams.

**Equipment:**
- Zig-zag air classifier (counter-current design)
- Cyclone separators (primary and secondary)
- Rotary airlock valves
- Centrifugal fan with VFD

**Parameters:**

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Air velocity (classifier column) | 7.5 m/s | 6.5–8.5 m/s | Fan VFD |
| Splitter gate position | 40% | 35–45% | Actuator position |
| Feed rate | 800 kg/h | 600–1,000 kg/h | Screw feeder |
| Static pressure (cyclone inlet) | −1.5 kPa | −1.0 to −2.0 kPa | Damper |

**Expected Streams:**

| Stream | Mass Fraction | Composition | Destination |
|--------|--------------|-------------|-------------|
| Hull stream (lights) | 25–30% | Hulls + fines | Hull process (milling) |
| Kernel stream (heavies) | 65–72% | Kernels + small hulls | Kernel process |
| Fines (dust) | 3–5% | Very fine hull/kernel | Dust collection |

**Quality Check: Separation Efficiency**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Hull purity (lights stream) | Every 2 hours | NIR / visual | ≥ 90% hull material | < 85% → adjust air velocity |
| Kernel carryover (lights) | Every 2 hours | Floatation test | ≤ 8% | > 10% → reduce splitter gap |
| Hull loss (heavies stream) | Every 4 hours | Density separation | ≤ 5% hull in heavies | > 8% → increase air velocity |

---

### 2.5 Hull Stream (Intermediate)

**Purpose:** Collect and convey the classified hull fraction to the milling stage.

**Equipment:**
- Surge hopper (500 kg)
- Magnet (CCP-1B, permanent rare-earth, ≥ 12,000 Gauss)
- Screw conveyor

**Parameters:**
- Conveying rate: 200–250 kg/h (matched to classifier output)
- Magnet cleaning frequency: Every shift
- Holdup time: ≤ 30 min

---

### 2.6 Milling

**Purpose:** Reduce hull particle size to target specification for powder applications.

**Equipment:**
- Pin mill (horizontal, dual-rotor counter-rotating)
- Hammermill (alternative for coarse grind)
- Mill feeder (loss-in-weight)

**Parameters:**

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Pin mill rotor speed | 6,000 rpm | 5,500–6,500 rpm | VFD |
| Screen aperture (hammermill) | 0.8 mm | 0.6–1.2 mm | Screen change |
| Feed rate | 200 kg/h | 150–250 kg/h | Loss-in-weight feeder |
| Mill inlet temperature | Ambient | 15–30°C | — |
| Mill outlet temperature | ≤ 45°C | 35–50°C | Monitor (cooling air if needed) |

**Process Notes:**
- Temperature at mill outlet must remain ≤ 50°C to prevent lignan degradation
- Pin mill produces finer, more uniform particle size than hammermill
- Mill screen condition must be checked weekly for wear

**Quality Check: Milling**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Particle size D90 | Every 2 hours | Laser diffraction | ≤ 250 µm | > 300 µm → tighten gap or change screen |
| Particle size D50 | Every 2 hours | Laser diffraction | 80–120 µm | Out of range → adjust mill parameters |
| Temperature after mill | Continuous | RTD sensor | ≤ 45°C | > 50°C → reduce feed rate or trip mill |
| Bulk density | Daily | Scott volumeter | 0.35–0.45 g/mL | Out of spec → check mill wear |

---

### 2.7 Sifting

**Purpose:** Classify milled hull powder by particle size; remove oversize particles for re-milling.

**Equipment:**
- Gyratory sifter (2-deck, 200 µm and 500 µm screens)
- Pneumatic conveying system
- Oversize return (re-grind loop)

**Parameters:**

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Top screen aperture | 500 µm | — | Fixed |
| Bottom screen aperture | 200 µm | — | Fixed |
| Sifter gyratory speed | 300 rpm | 280–320 rpm | VFD |
| Inclination angle | 5° | 3–7° | Manual adjustment |
| Feed rate | 200 kg/h | 150–250 kg/h | Screw feeder |

**Screen Fractions:**

| Fraction | Screen | Mass % | Handling |
|----------|--------|--------|----------|
| Overs (retained on top) | > 500 µm | 3–7% | Return to mill |
| Coarse (through top, retained on bottom) | 200–500 µm | 15–25% | Optional re-grind or coarser product |
| Fines (through bottom) | < 200 µm | 70–80% | Final hull powder |

**Quality Check: Sifting**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Overs in final product | Every 2 hours | Sieve (500 µm) | ≤ 1.0% | > 2.0% → check screen integrity |
| Screen integrity | Each shift | Visual + light test | No holes/tears | Replace damaged screen immediately |
| Sifter throughput | Continuous | Load cell | 150–250 kg/h | < 120 kg/h → check blinding |

---

### 2.8 Hull Powder (Final Product)

**Purpose:** Intermediate storage of finished hull powder awaiting packaging.

**Parameters:**
- Storage: Stainless steel bin, nitrogen-purged
- Hold time: ≤ 72 hours before packaging
- Temperature: 15–25°C
- Relative humidity: ≤ 40% in bin headspace

**Quality Check: Final Product (Before Packaging)**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Moisture | Every batch | Halogen moisture analyzer | ≤ 6.0% | > 6.5% → re-dry or reject |
| SDG lignan content | Every batch | HPLC | ≥ 2.5% (d.b.) | < 2.0% → identify root cause |
| Protein (N×6.25) | Every batch | Dumas | ≤ 18% | > 20% → check kernel carryover |
| Fat content | Every batch | NMR | 10–15% | Outside → report to R&D |
| Ash | Every batch | Muffle furnace (550°C) | ≤ 6.0% | > 7.0% → investigate hull purity |
| Aerobic plate count | Weekly | Petri film | ≤ 10,000 CFU/g | > 50,000 → production hold |
| Yeast & mold | Weekly | Petri film | ≤ 500 CFU/g | > 1,000 → production hold |
| Salmonella | Every 10 batches | PCR / culture | Negative/375g | Positive → quarantine + recall |
| E. coli / Coliforms | Weekly | MPN | < 3 MPN/g | ≥ 3 → investigate |
| Bulk density | Daily | Scott volumeter | 0.35–0.45 g/mL | Out → adjust mill |

---

### 2.9 Packaging (CCP-5)

**Purpose:** Package hull powder into finished goods under controlled conditions. **CCP-5: Metal Detection & Label Check.**

**Equipment:**
- Vertical form-fill-seal (VFFS) packaging machine
- Metal detector (conveyor, ≥ 1.0 mm ferrous, ≥ 1.5 mm non-ferrous, ≥ 2.0 mm stainless steel)
- Checkweigher (± 2 g accuracy)
- Label verification system (barcode scanner)
- Bag-in-box or bulk bag filler (as applicable)

**Parameters:**

| Parameter | Target | Range |
|-----------|--------|-------|
| Fill weight (retail) | 500 g | 495–505 g |
| Fill weight (bulk) | 20 kg | 19.9–20.1 kg |
| Seal temperature (VFFS) | 150°C | 145–155°C |
| Seal dwell time | 1.0 s | 0.8–1.2 s |
| Nitrogen flush (MAP) | 99.5% N₂ | ≥ 99.0% |
| Residual oxygen (MAP) | ≤ 2.0% | ≤ 3.0% |
| Metal detector rejection | Automatic | 100% inspected |

**Quality Check: Packaging**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Fill weight | Every 15 min | Scale check | Within spec | Reject ± off-weight packs |
| Seal integrity | Every hour | Visual + peel test | Continuous seal, no leaks | Any failure → adjust sealer |
| Metal detector function | Every hour | Test wands (Fe, NFe, SS) | All 3 detected | Functional check fail → line stop |
| Label accuracy | Every new SKU | Barcode scan | Match to batch | Mismatch → reject reels |
| Gas flush (MAP) | Every 30 min | Headspace O₂ analyzer | ≤ 2.0% O₂ | > 3.0% → adjust purge / reject |
| Package date/lot code | Every 15 min | Visual check | Legible, correct | Re-code or reject |

---

## 3. CCP Integration Matrix

| CCP ID | Process Stage | Hazard | Critical Limit | Monitoring | Corrective Action |
|--------|---------------|--------|----------------|------------|-------------------|
| **CCP-1A** | Cleaned Seed | Physical — Metal fragments | No metal > 1.0 mm Fe / 1.5 mm NFe / 2.0 mm SS | Magnet + metal detector, hourly test wands | Isolate last 30 min product; inspect and re-pass |
| **CCP-1B** | Hull Stream | Physical — Metal fragments | Same as CCP-1A | Reject mechanism verified hourly | Same as CCP-1A |
| **CCP-4** | Conditioning (Drying) | Biological — Pathogen survival | Product temp ≥ 60°C for ≥ 15 min | Continuous temp. recorder; manual check every 15 min | If temp drops: extend hold time or recondition |
| **CCP-5** | Packaging | Physical — Metal, Label mix-up | Metal detector functional; labels verified | CCP-5 log — every pack inspected | Reject all non-conforming packs; document |

---

## 4. Mass Balance (Per 1,000 kg Cleaned Seed Input)

| Stream | Mass (kg) | % of Input | Notes |
|--------|-----------|------------|-------|
| Cleaned seed in | 1,000 | 100% | Baseline |
| Moisture gain (conditioning) | +20 | +2.0% | Assuming 8% → 10% MC |
| Dehulling loss (dust, aspiration) | −15 | −1.5% | Fines to dust collection |
| Kernel stream (to kernel process) | −700 | −70.0% | Heavies from classifier |
| Hull stream (to milling) | 305 | 30.5% | Lights from classifier |
| Milling loss (dust, heat) | −10 | −1.0% | Mill aspiration |
| Sifting overs (return to mill) | −15 | −1.5% | Recirculated internally |
| Hull powder (final) | 280 | 28.0% | Finished product |

**Yield Targets:**
- Hull powder yield (from cleaned seed): **24–30%**
- Hull extraction efficiency: **≥ 88%** (hull in seed → hull in product)
- First-pass yield (no rework): **≥ 92%**

**Loss Points & Recovery:**
| Loss Point | Typical % | Recovery Method |
|------------|-----------|-----------------|
| Dust collection fines | 3–5% | Sold as animal feed ingredient |
| Kernel carryover in hulls | 5–8% | Recovered by adjusting classifier |
| Oversize re-mill loss | 1–2% | 85% returned to production |
| Packaging line waste | 0.5–1% | Start-up/shutdown purge |

---

## 5. Troubleshooting Guide

### 5.1 Conditioning Issues

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| Hulls sticking to kernels | Insufficient conditioning temp/time; low moisture | Increase steam temp to 68°C; verify 20 min hold; check moisture ≥ 9.5% |
| Seed overheating (> 72°C) | Steam pressure too high; bed too shallow | Reduce steam pressure; increase bed depth |
| Uneven conditioning | Channeling in tempering bin; clumping | Check bin discharge pattern; clean tempering bin; reduce fill level |

### 5.2 Dehulling Issues

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| Low dehulling efficiency (< 80%) | RPM too low; seed moisture high (> 11%); rolls worn | Increase RPM to 4,000+; re-check conditioning; replace rolls |
| Excessive fines (> 18%) | RPM too high; impact disc worn or imbalanced | Reduce RPM; inspect and balance disc; check for tramp metal damage |
| Kernel breakage (> 8%) | Roll gap too tight; impact too aggressive | Widen gap to 1.0 mm; reduce impact disc speed by 200 rpm |
| Mill plugging | Feed rate too high; seed sticky (over-conditioned) | Reduce feed rate; check conditioning temp ≤ 70°C |

### 5.3 Air Classification Issues

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| High kernel in hull stream (> 10%) | Air velocity too high; splitter gap too wide | Reduce fan speed 0.5 m/s steps; close splitter 2% |
| High hull loss to kernel stream (> 8%) | Air velocity too low; feed rate fluctuation | Increase fan speed; stabilize feed with loss-in-weight feeder |
| Cyclone plugging | High moisture (> 11%); sticky fines buildup | Reduce conditioning moisture; clean cyclone weekly; increase air velocity |

### 5.4 Milling & Sifting Issues

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| Coarse particle size (D90 > 300 µm) | Mill screen worn/blocked; feed rate too high | Replace screen; reduce feed rate; check pin wear |
| Mill overheating (> 50°C) | Feed too fast; dull pins/hammers; screen blinding | Reduce feed rate; replace wear parts; clean screen |
| Screen blinding (sifter) | High moisture or fat content; static buildup | Reduce milled product moisture; install antistatic brushes; increase gyratory speed |
| High oversize in final product | Screen tear; sifter bypass | Inspect/replace screen; check gasket seals |

### 5.5 Quality & Safety Issues

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| High moisture in final product (> 6.5%) | Insufficient drying; high ambient humidity; packaging in wet conditions | Verify conditioning; reduce conditioning moisture target; seal packaging area |
| SDG lignan below spec (< 2.0%) | High kernel carryover; variety change; bad incoming seed | Adjust classifier; check incoming seed analysis; contact supplier |
| Microbiological positive (Salmonella) | Cross-contamination; raw material issue; sanitation failure | Isolate batch; quarantine; deep clean line; investigate root cause |
| Metal detection rejects | Equipment wear (metal fragments); upstream metal | Identify source; inspect mill/dehuller for wear; replace worn parts |

---

## 6. Application Summary

### 6.1 Target Markets

| Market Segment | Typical Use Level | Key Benefit |
|----------------|-------------------|-------------|
| Bakery — bread, muffins, crackers | 3–10% of flour weight | Fiber boost, moisture retention, clean label |
| Cereal & granola | 5–15% | Crunchy texture, omega-3 claim support |
| Snack bars | 5–12% | Binding, fiber, nutty flavor |
| Plant-based meat analogs | 2–8% | Fiber, texture, water binding |
| Beverage powder blends | 3–7% | Dietary fiber, lignans |
| Dietary supplements (capsules/sachets) | 250–500 mg per serving | SDG lignan concentration |
| Pet food / animal feed | 2–5% | Fiber, coat health |

### 6.2 Formulation Guidelines

- **Water absorption:** Hull powder absorbs 3–4× its weight in water. Adjust liquid in formulations accordingly.
- **Flavor impact:** Mild nutty, slightly earthy. Best masked with chocolate, fruit, or spice profiles at > 8% inclusion.
- **Color:** Light to medium tan. Will affect color of white/light baked goods.
- **Shelf life:** 12 months when stored < 25°C, < 60% RH in sealed packaging.
- **Allergen status:** Flaxseed is not a priority allergen in most jurisdictions; however, facility may process tree nuts or soy — verify per location.
- **Labeling:** "Flaxseed hull powder" or "Flax hull fiber." SDG content may be declared separately.

### 6.3 Typical Nutritional Profile (per 100 g)

| Component | Typical Value | Method |
|-----------|--------------|--------|
| Energy | 350–400 kcal | Calculation |
| Protein | 14–18 g | Dumas (N×6.25) |
| Fat (total) | 10–15 g | NMR |
| — of which ALA | 4–6 g | GC-FID |
| Available carbohydrates | 5–10 g | Calculation by difference |
| Dietary fiber | 45–55 g | AOAC 991.43 |
| — of which soluble | 8–12 g | AOAC 991.43 |
| SDG lignan | 2.5–4.0 g | HPLC |
| Moisture | ≤ 6.0 g | Halogen |

---

## 7. References & Related Documents

| Document ID | Title |
|-------------|-------|
| PROD-HACCP-001 | HACCP Plan — Flaxseed Processing |
| PROD-KERNEL-001 | Flaxseed Kernel Processing Document |
| PROD-CLEAN-001 | Sanitation Standard Operating Procedures |
| QA-SPEC-FHP-001 | Hull Powder Finished Product Specification |
| QA-MICRO-001 | Microbiological Testing Schedule |
| LOG-RECEIVE-001 | Raw Material Receiving & Inspection Protocol |
| ENG-DEHULL-001 | Dehuller Maintenance & Calibration Manual |

---

> **Document owner:** Process Engineering Manager  
> **Approval required:** Operations Director, QA Director  
> **Review frequency:** Annual or upon process change
