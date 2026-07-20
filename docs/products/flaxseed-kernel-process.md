# Flaxseed Kernel Processing — Process & Workflow Document

> **Document ID:** PROD-KERNEL-001  
> **Version:** 1.0  
> **Last Updated:** 2026-07-20  
> **Product:** Flaxseed Kernel Products (Whole Kernel, Kernel Meal, Kernel Oil)

---

## 1. Process Overview

The flaxseed kernel process extracts the inner kernel (cotyledon) from dehulled flaxseed, producing kernel-rich streams for oil pressing or milling. The process prioritizes kernel integrity for whole-kernel applications and controlled particle size for meal and oil applications.

### 1.1 Process Flow Summary

```
Cleaned Seed → Conditioning → Dehulling → Air Classification
    → Kernel Stream → (Oil Pressing OR Milling) → QC → Packaging
```

### 1.2 High-Level Parameters

| Parameter | Target | Tolerance |
|-----------|--------|-----------|
| Kernel purity (from classifier) | ≥ 95% kernel | ±2% |
| Kernel yield (from cleaned seed) | 62–70% | ±3% |
| Moisture (kernel meal) | ≤ 7.0% | ±0.5% |
| Oil content (kernel meal, defatted) | ≤ 8% | ±1% |
| Particle size (meal, D90) | ≤ 500 µm | ±50 µm |

---

## 2. Detailed Process Stages

### 2.1 Cleaned Seed (Input)

**Purpose:** Receive and hold flaxseed that has passed through CCP-1 (Cleaning). Same receiving specs as hull process — see hull-process.md §2.1.

**Equipment:**
- Receiving hopper (2,000 kg)
- Destoner (gravity table)
- Magnet (CCP-1, ≥ 12,000 Gauss)
- Surge bin (5,000 kg)

**Parameters:**
- Foreign material: ≤ 0.5% (by weight)
- Dockage (chaff, weed seeds): ≤ 2.0%
- Moisture: 6.0–9.5%
- Temperature: Ambient

**Quality Check: Incoming Raw Material**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Variety/identity | Per lot | COA review | Match purchase spec | Mismatch → hold for R&D |
| Moisture | Per lot | NIR | 6.0–9.5% | > 10% → conditional acceptance with price adjustment |
| Oil content | Per lot | NMR | 38–44% | < 36% → reject or renegotiate |
| Free fatty acids (FFA) | Per lot | Titration | ≤ 1.0% oleic | > 1.5% → reject (rancidity risk) |
| Peroxide value (PV) | Per lot | Titration | ≤ 2.0 meq/kg | > 3.0 → reject |
| Visual defects | Every 50 bags | Visual inspection | ≤ 2% damaged seeds | > 5% → reject lot |
| Metal contamination | Continuous | CCP-1 magnet + detector | Zero detectable | Shut down; isolate 30 min product |

---

### 2.2 Conditioning

**Purpose:** Controlled heating and moisturizing to optimize hull separation. Kernel process conditioning may differ slightly from hull process to favor kernel intactness.

**Equipment:**
- Horizontal paddle conditioner (steam-injected)
- Tempering screw (jacketed, 10 min residence)
- Steam generator (2–3 bar, culinary grade)

**Parameters:**

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Conditioning temperature | 55°C | 50–60°C | Steam injection PID |
| Moisture after conditioning | 9.0% | 8.5–9.5% | Water spray + steam condensate |
| Residence time | 15 min | 12–18 min | Screw speed |
| Steam flow | 50 kg/h | 40–60 kg/h | Mass flow controller |
| Bed depth | 20 cm | 15–25 cm | Weir gate |

**Process Notes:**
- Kernel process uses **lower temperature** (55°C) than hull process (65°C) to preserve kernel integrity
- Excessive moisture (> 9.5%) leads to kernel softening and oil exudation in dehuller
- Steam quality must be culinary-grade — no boiler treatment chemicals

**Quality Check: Conditioning**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Temperature | Every 15 min | RTD probe | 50–60°C | > 62°C → reduce steam; < 48°C → increase |
| Moisture | Every batch | NIR | 8.5–9.5% | < 8.0% or > 10.0% → hold & adjust |
| Kernel firmness | Every hour | Manual squeeze test | Kernels intact, hull loose | Hull sticking → increase time or temp by 2°C |

---

### 2.3 Dehulling

**Purpose:** Gently separate hull from kernel while maximizing intact kernel yield.

**Equipment:**
- Rubber-roll dehuller (differential speed, soft rolls)
- Impact-free aspiration separator
- Rotary sifter (for kernel/hull pre-sort)

**Parameters:**

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Roll speed (fast roll) | 1,200 rpm | 1,100–1,300 rpm | VFD |
| Roll speed (slow roll) | 600 rpm | 550–650 rpm | VFD |
| Differential ratio | 2.0:1 | 1.8:1–2.2:1 | Fixed gear |
| Roll gap | 0.5 mm | 0.4–0.7 mm | Manual micrometer adjust |
| Feed rate | 600 kg/h | 500–700 kg/h | Screw feeder VFD |
| Aspiration velocity | 4 m/s | 3–5 m/s | Damper |

**Key Differences from Hull Process Dehuller:**
- Rubber rolls (vs. metal impact disc) — gentler on kernels
- Lower speed (1,200 vs. 3,800 rpm) — reduces breakage
- Narrower roll gap (0.5 vs. 0.8 mm) — compensates for lower impact force

**Quality Check: Dehulling**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Kernel integrity (whole) | Every hour | Hand sort (100 g) | ≥ 90% whole kernels | < 85% → reduce roll speed or widen gap |
| Dehulling efficiency | Every hour | Sieve + hand sort | ≥ 80% hull release | < 75% → increase differential speed |
| Fines generation | Every 2 hours | Sieve (< 1 mm) | ≤ 5% | > 8% → check roll condition |
| Rubber roll wear | Weekly | Visual + micrometer | ≥ 8 mm rubber remaining | < 5 mm → replace rolls |

---

### 2.4 Air Classification

**Purpose:** Separate kernel stream (heavy fraction) from hulls (light fraction). The kernel stream is the primary product for this process.

**Equipment:**
- Two-stage aspirator classifier
- Primary cyclone (kernel recovery)
- Secondary cyclone (fines collection)
- Rotary airlocks

**Parameters:**

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Primary air velocity | 6.0 m/s | 5.5–6.5 m/s | Fan VFD |
| Secondary air velocity | 8.0 m/s | 7.5–8.5 m/s | Damper |
| Splitter position | 60% | 55–65% | Actuator (heavies bias) |
| Feed rate | 600 kg/h | 500–700 kg/h | Screw feeder |

**Expected Streams:**

| Stream | Mass Fraction | Composition | Destination |
|--------|--------------|-------------|-------------|
| Kernel stream (heavies) | 72–78% | Kernels + trace hulls | Oil press or mill |
| Hull stream (lights) | 18–25% | Hull particles + fines | Hull process (milling) |
| Dust | 2–4% | Fine particles | Dust collection |

**Quality Check: Air Classification**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Kernel purity (heavies) | Every 2 hours | Density separation | ≥ 95% kernel | < 92% → reduce air velocity 0.3 m/s |
| Hull in kernel stream | Every 2 hours | Visual + density | ≤ 5% hulls | > 8% hulls → adjust classifier |
| Kernel loss to hull stream | Every 4 hours | Sieve + weighing | ≤ 3% of total kernel | > 5% → reduce secondary air velocity |

---

### 2.5 Kernel Stream (Intermediate)

**Purpose:** Collect, optionally size-grade, and convey kernels to downstream processing (oil pressing or milling).

**Equipment:**
- Surge hopper (1,000 kg)
- Rotary sizer (optional, vibratory)
- Metal detector (CCP-1B)
- Pneumatic or mechanical conveyor

**Options — Size Grading (If Required for Whole Kernel Market):**

| Grade | Screen Size | Typical % of Kernel | Application |
|-------|-------------|---------------------|-------------|
| Whole kernel (grade A) | > 3.5 mm | 40–50% | Retail, snack, bakery topping |
| Split kernel (grade B) | 2.0–3.5 mm | 30–40% | Milling, coarse meal |
| Fines | < 2.0 mm | 10–20% | Milling (meal), oil press |

**Quality Check: Kernel Stream**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Kernel moisture | Every batch | NIR | 8.0–9.5% | > 10% → reduce conditioning spray |
| Hull content | Every 2 hours | Density separation | ≤ 5% | > 8% → adjust classifier |
| Color / visual | Every hour | Visual (L*a*b* reference) | Light yellow-tan | Darkening → check for overheating in conditioning |

---

## 3. Downstream Processing — Dual Path

The kernel stream can be directed to **one of two parallel processing lines** depending on the target product:

---

### Path A: Oil Pressing

**Purpose:** Extract flaxseed oil from kernels, producing crude oil and press cake (kernel meal).

#### 3A.1 Kernel Pre-Heat

**Equipment:** Vertical stack cooker (3-tray, steam-heated)

| Parameter | Target | Range |
|-----------|--------|-------|
| Pre-heat temperature | 90°C | 85–95°C |
| Residence time | 20 min | 15–25 min |
| Moisture after cook | 5.0% | 4.5–5.5% |

**Purpose:** Reduce moisture, denature enzymes, increase oil fluidity.

#### 3A.2 Screw Pressing

**Equipment:** Single-screw expeller press (e.g., Anderson Duo or equivalent)

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Screw speed | 25 rpm | 20–30 rpm | VFD |
| Barrel temperature | 80°C | 75–85°C | Jacket heating/cooling |
| Choke gap | 8 mm | 6–10 mm | Manual adjust |
| Throughput | 500 kg/h | 400–600 kg/h | Feeder speed |
| Motor load | 80% | 70–90% | Amp meter |

**Expected Outputs:**

| Stream | Mass % | Composition |
|--------|--------|-------------|
| Crude oil | 30–35% | Oil + meal fines |
| Press cake | 65–70% | Meal, 8–12% residual oil |

**Quality Check: Pressing**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Residual oil in cake | Every 2 hours | NMR | ≤ 12% | > 15% → tighten choke or reduce speed |
| Oil temperature | Continuous | In-line RTD | ≤ 50°C (exit) | > 55°C → activate cooler |
| Cake moisture | Every 2 hours | Halogen | ≤ 7.0% | > 8.0% → reduce feed or increase cooking temp |

#### 3A.3 Oil Filtration

**Equipment:** Plate-and-frame filter press, polish filter

| Parameter | Target | Range |
|-----------|--------|-------|
| Filter aid (diatomaceous earth) | 0.5% w/w | 0.3–0.8% |
| Pressure (max) | 4 bar | 3–5 bar |
| Temperature | 35°C | 30–40°C |

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Oil clarity | Every batch | Visual | Clear, no sediment | Turbid → re-filter |
| FFA in oil | Every batch | Titration | ≤ 0.5% | > 1.0% → reprocess or downgrade |
| PV in oil | Every batch | Titration | ≤ 1.0 meq/kg | > 2.0 → reject for human consumption |
| Sediment after filtration | Every batch | Centrifuge test | ≤ 0.1% | > 0.2% → re-filter with tighter media |

---

### Path B: Milling (Kernel Meal)

**Purpose:** Produce kernel meal (full-fat or partially defatted) for bakery, supplement, and feed applications.

#### 3B.1 Hammer Milling

**Equipment:** Hammermill with DSA (dynamic screen assist)

| Parameter | Target | Range | Control Method |
|-----------|--------|-------|----------------|
| Screen aperture | 1.5 mm | 1.0–2.0 mm | Screen selection |
| Rotor speed | 3,000 rpm | 2,800–3,200 rpm | VFD |
| Feed rate | 400 kg/h | 300–500 kg/h | Feeder VFD |
| Mill temperature | ≤ 45°C | 35–50°C | Cooling air |

**Quality Check: Milling**

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Particle size D90 | Every 2 hours | Sieve shaker | ≤ 500 µm | > 600 µm → change screen or reduce feed |
| Temperature out | Continuous | RTD | ≤ 45°C | > 50°C → reduce feed or activate cooling |
| Bulk density | Daily | Scott cup | 0.45–0.55 g/mL | Out of spec → adjust hammer configuration |

#### 3B.2 Optional: Defatting (Partial)

**Purpose:** Reduce oil content in meal for specific customer requirements.

**Method:** Mechanical pressing (Path A) → then press cake is milled.

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Residual oil | Per batch | NMR | ≤ 8% (defatted) | > 10% → re-press |
| Protein (defatted meal) | Per batch | Dumas | ≥ 30% | < 28% → investigate kernel purity |

---

## 4. QC — Final Product Testing

### 4.1 Whole Kernel (Unmilled) — Final QC

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Moisture | Every batch | Halogen | ≤ 8.0% | > 9.0% → re-dry |
| Purity (kernels only) | Every batch | Hand sort | ≥ 98% | < 95% → re-classify |
| Whole kernels | Every batch | Sieve (3.5 mm) | ≥ 85% | Varies by grade |
| Color | Every batch | Visual (reference) | Light yellow | Dark → check conditioning |
| FFA (kernel oil) | Per batch | Titration | ≤ 1.0% | > 1.5% → reject |
| PV (kernel oil) | Per batch | Titration | ≤ 2.0 meq/kg | > 3.0 → reject |

### 4.2 Kernel Meal (Milled) — Final QC

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| Moisture | Every batch | Halogen | ≤ 7.0% | > 8.0% → re-dry |
| Protein | Every batch | Dumas (N×6.25) | 20–24% (full-fat) / ≥ 30% (defatted) | Out → report |
| Fat | Every batch | NMR | 38–44% (full-fat) / ≤ 8% (defatted) | Out → check upstream |
| Fiber | Every batch | AOAC | ≤ 8% | > 10% → hull contamination |
| Particle size D90 | Every batch | Sieve | ≤ 500 µm | > 600 µm → re-mill |
| APC | Weekly | Petri film | ≤ 10,000 CFU/g | > 50,000 → hold |
| Yeast & mold | Weekly | Petri film | ≤ 500 CFU/g | > 1,000 → hold |
| Salmonella | Every 10 batches | PCR/culture | Negative/375g | Positive → quarantine + recall |

### 4.3 Kernel Oil (Pressed) — Final QC

| Check | Frequency | Method | Target | Action Limit |
|-------|-----------|--------|--------|-------------|
| FFA | Every batch | AOCS Ca 5a-40 | ≤ 0.5% | > 1.0% → downgrade to industrial |
| PV | Every batch | AOCS Cd 8-53 | ≤ 1.0 meq/kg | > 2.0 → reject |
| p-Anisidine value | Every batch | AOCS Cd 18-90 | ≤ 5.0 | > 10 → oxidation concern |
| ALA content | Per supplier lot | GC-FID | ≥ 52% | < 48% → verify variety/ origin |
| Color (Lovibond) | Every batch | Lovibond tintometer | ≤ 1.5R, ≤ 15Y | Out → check bleaching |
| Flavor score | Every batch | Sensory panel | ≥ 6/10 | < 5 → reprocess or blend |
| Cold test | Every batch | AOCS Cc 11-53 | Pass (5.5 h at 0°C) | Fail → winterize |

---

## 5. CCP Integration

| CCP ID | Process Stage | Hazard | Critical Limit | Monitoring | Corrective Action |
|--------|---------------|--------|----------------|------------|-------------------|
| **CCP-1** | Cleaned Seed (Receiving) | Physical — Metal | No metal > 1.0 mm Fe / 1.5 mm NFe / 2.0 mm SS | Magnet + metal detector; hourly wand test | Isolate 30 min of product; clean magnetic separator |
| **CCP-1B** | Kernel Stream (Intermediate) | Physical — Metal | Same as CCP-1 | Reject mechanism; hourly test | Same as CCP-1 |
| **CCP-4** | Conditioning | Biological — Pathogen survival | Product ≥ 50°C for ≥ 15 min | Continuous temp recording; manual check every 15 min | If below: extend hold or recondition |
| **CCP-4B** | Pre-Heat (Oil Press) | Biological — Pathogen reduction | Product ≥ 85°C for ≥ 10 min | Temp chart recorder; operator log | Extend residence time or raise temp |
| **CCP-5** | Packaging | Physical — Metal, Label | Metal detector functional; label match | CCP-5 checklist; 100% inspection | Reject non-conforming packs |

---

## 6. Mass Balance (Per 1,000 kg Cleaned Seed Input)

### Path A: Oil Pressing

| Stream | Mass (kg) | % of Input | Notes |
|--------|-----------|------------|-------|
| Cleaned seed | 1,000 | 100% | Baseline |
| Conditioning moisture gain | +15 | +1.5% | 8% → 9% MC |
| Dehulling loss | −10 | −1.0% | Fines to dust |
| Hull stream (to hull milling) | −220 | −22.0% | From classifier |
| Kernel stream to press | 785 | 78.5% | Includes ~5% hull residue |
| Pre-heat moisture loss | −20 | −2.0% | 9% → 5% MC |
| Crude oil (pressed) | 255 | 25.5% | 32.5% of kernel stream |
| Press cake (kernel meal) | 510 | 51.0% | 65% of kernel stream |
| Oil filtration loss | −5 | −0.5% | Filter aid + sediment |
| **Refined oil (final)** | **250** | **25.0%** | |
| **Kernel meal (final)** | **510** | **51.0%** | ~10% residual oil |

### Path B: Milling Only

| Stream | Mass (kg) | % of Input | Notes |
|--------|-----------|------------|-------|
| Cleaned seed | 1,000 | 100% | |
| Conditioning moisture gain | +15 | +1.5% | |
| Dehulling / classifier losses | −20 | −2.0% | Dust, fines |
| Hull stream (to hull milling) | −220 | −22.0% | |
| Kernel stream to mill | 775 | 77.5% | |
| Mill dust loss | −15 | −1.5% | |
| **Kernel meal (final)** | **760** | **76.0%** | Full-fat, 38–44% oil |

### Yield Targets

| Product | Target Yield | First-Pass Yield |
|---------|-------------|------------------|
| Whole kernels (from seed) | 40–50% | ≥ 90% |
| Kernel meal (full-fat, from seed) | 74–78% | ≥ 92% |
| Kernel meal (defatted, from seed) | 48–54% | ≥ 90% |
| Kernel oil (from seed) | 23–27% | ≥ 88% |

### Loss Points & Recovery

| Loss Point | Typical % | Recovery Method |
|------------|-----------|-----------------|
| Dehulling fines | 1–2% | Sold as feed ingredient |
| Hull stream (kernel loss) | 2–3% | Recovered by classifier adjustment |
| Press cake fines | 0.5–1% | Blended back into meal |
| Oil filter sludge | 0.3–0.5% | Sold for industrial use |
| Packaging waste | 0.3–0.8% | Reprocessed as lower-grade meal |

---

## 7. Troubleshooting Guide

### 7.1 Conditioning & Dehulling

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| Low kernel recovery (< 72%) | Hulls not separating; kernels breaking | Reduce conditioning temp to 52°C; increase kernel-side classifier air velocity; check rubber roll condition |
| High hull in kernel stream (> 8%) | Air classifier velocity too low; splitter wrong | Increase primary air velocity by 0.5 m/s; adjust splitter toward heavies |
| High kernel breakage (> 15%) | Rubber rolls worn; gap too tight; feed too fast | Replace rolls (check mic); widen gap to 0.6 mm; reduce feed to 500 kg/h |
| Rubber roll glazing/overheating | Differential speed too low; gap too tight | Increase differential ratio; widen roll gap; ensure uniform feed distribution |

### 7.2 Oil Pressing (Path A)

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| Low oil yield (< 28%) | Kernel moisture too high (> 6%); pre-heat temp low | Reduce moisture in pre-heat step; increase cooker temperature to 95°C; tighten choke gap |
| High residual oil in cake (> 15%) | Press choke too loose; screw speed too fast | Tighten choke 1 mm; reduce screw speed 2 rpm; check barrel wear |
| Dark oil color | Overheating in press; high FFA in input | Reduce barrel temperature; verify incoming FFA ≤ 1.0%; clean press barrel |
| Oil turbidity after filtration | Filter media worn; pressure too high | Replace filter cloth; reduce pressure to ≤ 3 bar; check pre-coat |
| High FFA in oil (> 1.0%) | Kernel deterioration; long hold times | Reduce kernel hold time before pressing; lower pre-heat temperature; check seed quality |

### 7.3 Milling (Path B)

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| Coarse meal (D90 > 600 µm) | Screen worn or blown; hammer wear | Replace screen; reverse/replace hammers; reduce feed rate |
| Mill plugging | Oil-rich kernels smearing on screen; high moisture | Reduce kernel oil content (de-fat first); chill kernels to 10°C; use larger screen (2.0 mm) |
| Meal temperature > 50°C | Mill working too hard; screen blinding | Reduce feed; increase cooling air; clean screen with air blast |
| High hull content in meal (> 10%) | Air classifier not separating well; screen wear on classifier | Adjust classifier; check classifier screen integrity |

### 7.4 Quality & Microbiological

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| High APC (> 50,000 CFU/g) | Sanitation lapse; warm moist conditions; long hold times | Deep clean line; reduce kernel hold time; verify CCP-4 conditions; increase product rotation |
| Salmonella positive | Raw material contamination; sanitation failure; cross-contamination | Quarantine batch; trace raw material; fumigate area; intensifiy cleaning frequency |
| Rancid odor in meal/oil | High FFA or PV; prolonged storage; light exposure | Adjust storage (25°C max, dark, N₂ blanket); reduce hold times; test incoming seed PV |
| ALA below spec in oil | Variety change; adulteration; oxidation | Check supplier COA; test incoming seed; verify GC method |

### 7.5 Packaging & Metal Detection

| Problem | Possible Causes | Solutions |
|---------|----------------|----------|
| Metal detector false rejects | Static electricity; product effect (conductivity); vibration | Install static eliminator; re-calibrate product effect phase; stabilize conveyor |
| Seal failure (bags) | Temperature too low/high; contaminated seal area | Adjust seal temp ±5°C; check seal jaws for residue; verify packaging material spec |
| Weight variation (checkweigher) | Product density variation; faulty load cell | Check bulk density (adjust mill if needed); calibrate load cell; verify free-flow |

---

## 8. Application Summary

### 8.1 Whole Kernel Applications

| Application | Use Level | Benefit |
|-------------|-----------|---------|
| Bakery toppings (bread, bagels) | 3–8% | Crunch, visual, omega-3 |
| Trail mixes & granola | 5–15% | Nutrition, texture |
| Snack bars (pressed into bars) | 5–12% | Binding, ALA content |
| Retail packaged kernels | 100% | Direct consumption |

### 8.2 Kernel Meal Applications

| Application | Use Level | Benefit |
|-------------|-----------|---------|
| Bakery — bread, muffins, pancakes | 5–15% of flour | Protein & fiber boost, moist crumb |
| Gluten-free baking | 5–20% | Structure, nutrition |
| Smoothie & supplement blends | 10–25 g/serving | ALA omega-3, fiber, protein |
| Plant-based meat extenders | 3–10% | Texture, water binding, protein |
| Pet food & animal feed | 2–8% | Omega-3 enrichment, coat health |
| Nutritional supplements | 5–15 g/serving | Ground flaxseed functionality |

### 8.3 Kernel Oil Applications

| Application | Use Level | Benefit |
|-------------|-----------|---------|
| Dietary supplements (softgels, liquid) | 1,000–3,000 mg/day | ALA omega-3 (≥ 52%) |
| Functional foods — dressings, dips | 5–20% | Omega-3 enrichment |
| Personal care (creams, balms) | 2–10% | Emollient, skin barrier |
| Paints & varnishes (industrial) | 10–30% | Drying oil, renewable |

### 8.4 Formulation Guidelines

- **Whole kernels:** Maximum particle size 3.5–5.0 mm; toasting at 120–150°C for 8–15 min enhances flavor.
- **Kernel meal:** Water-holding capacity ~2:1 (meal:water). Adjust hydration in baked goods. Store at ≤ 25°C, ≤ 60% RH. Shelf life: 6 months (full-fat), 12 months (defatted).
- **Kernel oil:** Sensitive to light, heat, and oxygen. Store under nitrogen in opaque containers. Refrigerate after opening. Shelf life: 12 months (unopened, refrigerated).
- **Allergen status:** Flaxseed is not a major allergen in most jurisdictions. Facility may process other seeds/nuts — verify per site.

### 8.5 Typical Nutritional Profile

| Component | Whole Kernel | Kernel Meal (Full-Fat) | Kernel Oil |
|-----------|-------------|----------------------|------------|
| Energy (kcal/100g) | 530–550 | 520–540 | 884 |
| Protein (g/100g) | 20–24 | 22–26 | 0 |
| Fat (g/100g) | 38–44 | 38–44 | 99.9 |
| — ALA (g/100g) | 20–24 | 20–24 | 52–60 |
| Carbohydrates (g/100g) | 5–10 | 5–10 | 0 |
| Dietary fiber (g/100g) | 6–8 | 7–9 | 0 |
| Moisture (g/100g) | ≤ 8.0 | ≤ 7.0 | ≤ 0.1 |

---

## 9. Related Documents

| Document ID | Title |
|-------------|-------|
| PROD-HULL-001 | Flaxseed Hull Processing Document |
| PROD-HACCP-001 | HACCP Plan — Flaxseed Processing |
| PROD-CLEAN-001 | Sanitation Standard Operating Procedures |
| QA-SPEC-FKM-001 | Kernel Meal Finished Product Specification |
| QA-SPEC-FKO-001 | Kernel Oil Finished Product Specification |
| QA-SPEC-WKF-001 | Whole Kernel Flax — Product Specification |
| QA-MICRO-001 | Microbiological Testing Schedule |
| LOG-RECEIVE-001 | Raw Material Receiving & Inspection Protocol |
| ENG-PRESS-001 | Oil Press Maintenance & Calibration Manual |
| ENG-MILL-001 | Hammermill Maintenance & Calibration Manual |

---

> **Document owner:** Process Engineering Manager  
> **Approval required:** Operations Director, QA Director  
> **Review frequency:** Annual or upon process change
