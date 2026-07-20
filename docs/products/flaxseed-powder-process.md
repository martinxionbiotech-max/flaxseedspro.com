# Flaxseed Powder — Process & Workflow Document

**Document ID:** PROD-PROC-001  
**Version:** 1.0  
**Effective Date:** 2026-07-20  
**Product:** Flaxseed Powder (Full-Fat & Defatted)

---

## 1. Process Overview

The flaxseed powder manufacturing line converts cleaned flaxseed kernels (or whole seed) into a shelf-stable, finely milled powder. Two distinct process lines exist: **Full-Fat** and **Defatted**. The core flow is shared but key parameter differences are noted in each section below.

### Process Flow Diagram

```
Kernel / Whole Seed
       ↓
  Metal Detection (CCP-5)
       ↓
  Milling (Hammer / Pin / Cryo)
       ↓
     Sifting
       ↓
  N₂ Flush & Blending
       ↓
  Metal Check (CCP-5)
       ↓
    Packaging
```

---

## 2. Detailed Process Steps

### 2.1 Kernel / Whole Seed Receiving & Pre-Cleaning

| Parameter | Full-Fat Line | Defatted Line |
|-----------|--------------|---------------|
| Seed source | Brown/golden flaxseed kernels | Defatted flaxseed meal from oil press |
| Moisture spec | ≤8.0% | ≤6.0% |
| Foreign matter | ≤0.5% | ≤1.0% |
| Pre-cleaning | Air classifier + magnet | Vibrating screen + magnet |

- **Quality Gate:** Visual inspection per batch — no mold, insect damage, or off-odor.
- **Defatted:** Meal is received from the screw press (see oil-process.md), typically with 8–12% residual oil.

### 2.2 Metal Detection — CCP-5

| Parameter | Value |
|-----------|-------|
| Detection threshold | Fe ≥1.0 mm, Non-Fe ≥1.5 mm, SS ≥2.0 mm |
| Reject mechanism | Pneumatic diverter gate |
| Calibration frequency | Every 2 hours (with test wands) |
| Deviation limit | ≤1 reject per 1000 kg |

- **CCP-5:** Metal detection is the controlling critical control point for physical hazards.
- **Corrective action:** Reject contaminated batch; recalibrate detector; record in CCP log.
- **Monitoring:** Continuous with auto-reject; verified every 30 min by operator.

### 2.3 Milling

Three mill types are available depending on target particle size and product specification.

#### 2.3.1 Hammer Mill (Standard, Full-Fat & Defatted)

| Parameter | Range / Typical |
|-----------|----------------|
| Rotor speed | 2,800 – 3,600 RPM |
| Screen aperture | 0.8 – 3.0 mm |
| Tip speed | 80 – 120 m/s |
| Throughput | 300 – 800 kg/hr (depends on screen size) |
| Motor power | 30 – 55 kW |

- **Particle size control:** Smaller screen aperture → finer powder. A 0.8 mm screen produces ~200 mesh; 1.5 mm → ~100 mesh; 3.0 mm → ~60 mesh.
- **Full-Fat line:** Pre-chill kernels to 4–10°C to prevent heat buildup and oil smear.

#### 2.3.2 Pin Mill (Ultra-Fine, Full-Fat)

| Parameter | Range / Typical |
|-----------|----------------|
| Rotor speed | 6,000 – 12,000 RPM |
| Pin disc diameter | 300 – 600 mm |
| Airflow | 500 – 1,500 m³/hr (pneumatic conveying) |
| Throughput | 100 – 400 kg/hr |
| Product temperature at outlet | ≤45°C |

- **Particle size control:** Higher RPM → finer particles. At 10,000+ RPM, D50 reaches 30–50 µm (~300 mesh).
- **Note:** Suitable for full-fat only when combined with cooling air. Not recommended for defatted (high fines → dust explosion risk).

#### 2.3.3 Cryogenic Mill (Premium, Full-Fat)

| Parameter | Range / Typical |
|-----------|----------------|
| Grinding temperature | −150°C (liquid N₂ injection) |
| N₂ consumption | 1.5 – 2.5 kg N₂ per kg product |
| Mill type | Impact mill (pin or hammer) enclosed in cryogenic shroud |
| Throughput | 80 – 200 kg/hr |
| Product temperature at outlet | ≤−20°C |

- **Particle size:** D50 = 20–40 µm (~400 mesh) achievable without thermal degradation.
- **Advantages:** Preserves omega-3 fatty acids; prevents oil smear and screen clogging; extends shelf life by 30–50%.
- **Cost factor:** Cryogenic milling adds $0.30–0.60/kg to production cost.
- **Quality Gate:** Verify mill chamber temperature via thermocouple every 15 min.

### 2.4 Sifting

| Parameter | Value |
|-----------|-------|
| Sieve mesh | 60 – 200 mesh (depending on target) |
| Sieve type | Gyratory or tumbler sifter |
| Oversize recycle | Returns to mill hopper |
| Throughput | Matches mill output |

- **Quality Gate:** Sieve analysis every 30 min — 95% passing target mesh.
- **Target mesh table:**

| Powder Grade | Target Mesh | Typical D50 | Application |
|-------------|-------------|-------------|-------------|
| Coarse | 60 mesh | 250 µm | Baking, bulk blends |
| Standard | 80 mesh | 180 µm | General food ingredient |
| Fine | 100 mesh | 150 µm | Smoothies, beverages |
| Ultra-fine | 200 mesh | 75 µm | Nutritional supplements |

### 2.5 N₂ Flush & Blending

| Parameter | Full-Fat Line | Defatted Line |
|-----------|--------------|---------------|
| Residual O₂ in headspace | ≤2.0% | ≤3.0% |
| N₂ purity | ≥99.9% | ≥99.5% |
| Blending time | 5 – 10 min (ribbon blender) | 3 – 5 min |
| Temperature after blending | ≤35°C | ≤30°C |

- **Purpose:** Displace oxygen to prevent lipid oxidation (full-fat is more susceptible).

### 2.6 Metal Check — CCP-5 (Final)

| Parameter | Value |
|-----------|-------|
| Detection threshold | Fe ≥0.8 mm, Non-Fe ≥1.2 mm, SS ≥1.5 mm |
| Reject mechanism | Pneumatic pusher on conveyor |
| Verification | Test wand every 2 hours |

- **Critical limit:** Any ferrous metal >0.8 mm triggers rejection.
- **Record keeping:** All reject events logged with batch ID, time, and corrective action.

### 2.7 Packaging

| Parameter | Full-Fat Line | Defatted Line |
|-----------|--------------|---------------|
| Pack sizes | 0.5 – 25 kg (multiwall kraft + PE liner) | 10 – 25 kg |
| Gas flushing | N₂ (optional for retail pouches) | Not required |
| Seal integrity | Vacuum decay test every 100 packs | Visual check |
| Shelf life (declared) | 12 months (ambient) | 18 months |

---

## 3. Quality Gates (In-Process Checks)

| Check | Frequency | Method | Acceptable Limit | Action if Out of Spec |
|-------|-----------|--------|------------------|----------------------|
| Mill outlet temperature | Every 30 min | Infrared thermometer | ≤45°C (≤30°C for defatted) | Reduce feed rate, check cooling |
| Particle size (sieve) | Every 30 min | Ro-tap sieve shaker | 95% passing target mesh | Adjust screen/RPM, re-mill oversize |
| Peroxide Value (PV) | Every 30 min (full-fat) | AOCS Cd 8-53 | ≤2.0 meq O₂/kg | Divert to defatted line, check N₂ supply |
| Moisture content | Every 30 min | Halogen moisture analyzer | ≤6.0% (full-fat), ≤5.0% (defatted) | Adjust drying parameters |
| Metal detector test | Every 2 hours | Test wands (Fe, Non-Fe, SS) | All detected and rejected | Recalibrate, hold product since last OK test |
| Color (visual) | Every hour | Visual standard (L*a*b* optional) | Consistent with reference | Check for scorching, adjust mill speed |

---

## 4. CCP Integration Summary

| CCP Code | Hazard Type | Control Point | Critical Limit | Monitoring |
|----------|-------------|---------------|----------------|------------|
| CCP-4 | Biological (moisture) | Pre-mill drying / moisture control | Moisture ≤8.0% | In-line moisture meter every 30 min |
| CCP-5 | Physical (metal) | Inlet metal detector + final metal check | Fe ≥1.0 mm / ≥0.8 mm | Continuous + test wand every 2 hr |

---

## 5. Troubleshooting

### 5.1 Overheating During Milling

| Possible Cause | Check | Solution |
|---------------|-------|----------|
| Feed rate too high | Mill amperage draw | Reduce feed rate by 10–20% |
| Screen clogged | Pressure drop across screen | Replace or clean screen |
| Insufficient cooling air | Airflow meter | Increase airflow or check ducting |
| Blunt hammers/pins | Visual wear pattern | Replace wear parts |
| High ambient temp | Room thermometer | Pre-cool feedstock to ≤10°C |

### 5.2 Poor Grind (Inconsistent Particle Size)

| Possible Cause | Check | Solution |
|---------------|-------|----------|
| Worn screen / pin disc | Visual inspection | Replace worn parts |
| Wrong screen aperture | Screen spec tag | Install correct screen |
| Variable feed rate | Feed hopper level | Ensure consistent feed (vibratory feeder) |
| Moisture > 8% | Moisture analyzer | Pre-dry seed to ≤8% |
| RPM too low | Tachometer reading | Increase to target RPM range |

### 5.3 High Peroxide Value (PV > 2.0 meq/kg)

| Possible Cause | Check | Solution |
|---------------|-------|----------|
| Mill temperature too high | Product outlet temp | Reduce mill speed, increase cooling |
| High O₂ in headspace | Headspace O₂ analyzer | Increase N₂ flow rate |
| Old feedstock | Raw material age | Use fresher seed (≤6 months old) |
| Metal contamination (pro-oxidant) | Metal detector | Check for wear metal in product |
| Cryo mill — insufficient N₂ | N₂ flow meter | Increase N₂:product ratio to ≥1.5:1 |

### 5.4 Clogging / Screen Blinding

| Possible Cause | Check | Solution |
|---------------|-------|----------|
| Oil smear (full-fat, temp > 40°C) | Mill outlet temp | Pre-chill seed, reduce RPM |
| High moisture (> 8%) | Moisture analyzer | Dry seed before milling |
| Screen aperture too small | Screen spec | Use larger aperture (e.g., 1.5 mm) |
| Feed rate too high | Mill load amps | Reduce feed rate |
| Fine recirculation buildup | Oversize return line | Clean recirculation path |

### 5.5 High Fines / Dust (Defatted Line)

| Possible Cause | Check | Solution |
|---------------|-------|----------|
| Hammer mill speed too high | RPM reading | Reduce to 2,800–3,000 RPM |
| Screen too fine | Screen size | Increase to ≥1.5 mm |
| Meal too dry | Moisture analyzer | Target 5–6% moisture |
| Inadequate dust collection | Baghouse differential pressure | Clean or replace filter bags |

---

## 6. Line-Specific Differences — Full-Fat vs. Defatted

| Aspect | Full-Fat Line | Defatted Line |
|--------|--------------|---------------|
| Feedstock | Whole flaxseed or kernel | Press cake (8–12% residual oil) |
| Pre-milling cooling | Required (chill to 4–10°C) | Not required |
| Mill type | Hammer, pin, or cryo | Hammer mill only |
| Temperature sensitivity | High (oil oxidation risk) | Moderate |
| N₂ flushing | Required | Optional |
| Target particle size | 100–200 mesh | 60–100 mesh |
| Shelf life | 12 months | 18 months |
| PV monitoring | Every 30 min | Every 60 min |
| Dust explosion risk | Low (oil suppresses dust) | Higher (dry, fine particles) |

---

## 7. Equipment List

| Equipment | Specification | Supplier Options |
|-----------|--------------|-----------------|
| Hammer mill | 30–55 kW, 2800–3600 RPM | Fitzpatrick, Hosokawa |
| Pin mill | 15–30 kW, 6000–12000 RPM | Alpine, Kemutec |
| Cryogenic mill | LN₂ injection, −150°C | Air Products, Messer |
| Sifter / screener | Gyratory, 60–200 mesh | Sweco, Russell |
| Ribbon blender | 500–2000 kg capacity | Munson, ASCO |
| N₂ generator | ≥99.9% purity, 50–200 Nm³/hr | Atlas Copco, Parker |
| Metal detector (inlet) | Pipeline, Fe ≥1.0 mm | Eriez, Loma |
| Metal detector (final) | Conveyor, Fe ≥0.8 mm | Mettler-Toledo, Loma |
| Packaging machine | VFFS or pre-made bags | Bosch, Ishida |

---

## 8. References

- AOCS Cd 8-53 — Peroxide Value, Acetic Acid-Chloroform Method
- ISO 2070 — Determination of particle size by sieving
- CCP-4 & CCP-5 Standard Operating Procedures (see QMS-SOP-004/005)
- Flaxseed Powder Product Specification — PROD-SPEC-001

---

*End of Document — Flaxseed Powder Process Flow*
