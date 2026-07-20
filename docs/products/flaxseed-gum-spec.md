# Flaxseed Gum — Technical Product Specification

**Product Name:** Flaxseed Gum (Linum usitatissimum)
**Product Code:** FSP-GUM-001
**Document ID:** FSP-GUM-SPEC-001
**Version:** 1.0
**Issue Date:** July 20, 2026
**Supersedes:** New Document

---

## 1. Product Description

Flaxseed Gum (FSP-GUM-001) is a high-purity, natural polysaccharide complex extracted from whole flaxseed (Linum usitatissimum L.) via aqueous extraction, ethanol precipitation, and spray-drying. It is a light-tan to off-white free-flowing powder with a bland, neutral taste and no distinct odor. The gum is composed primarily of acidic arabinoxylans with a high molecular weight distribution, conferring exceptional water-binding, thickening, emulsifying, and stabilizing properties. This product is suitable for food, nutraceutical, cosmetic, and pharmaceutical applications where clean-label hydrocolloid functionality is required.

---

## 2. Proximate Analysis

| Parameter                | Specification       | Method                     |
|--------------------------|---------------------|----------------------------|
| Total Polysaccharide     | 75 – 85 %           | Phenol-Sulfuric Acid (AOAC)|
| Protein (N × 6.25)       | 3.0 – 6.0 %         | AOAC 984.13 (Kjeldahl)     |
| Uronic Acid              | 8 – 14 %            | _m_-Hydroxydiphenyl Method |
| Moisture                 | ≤ 5.0 %             | AOAC 925.10 (Vacuum Oven)  |
| Ash                      | 4.0 – 7.0 %         | AOAC 923.03 (525 °C)       |
| Acetyl Groups            | 2.0 – 4.0 %         | HPLC                       |

**Total Carbohydrates (by difference):** ≥ 80 %

**pH (1 % w/w aqueous solution, 25 °C):** 5.5 – 7.5

---

## 3. Monosaccharide Profile

The polysaccharide backbone and side-chain composition are determined by HPLC after complete acid hydrolysis (2 M TFA, 121 °C, 2 h). Seven neutral monosaccharides are routinely quantified.

| Monosaccharide | Composition (% w/w) |
|----------------|---------------------|
| Xylose         | 30 – 38             |
| Galactose      | 20 – 28             |
| Rhamnose       | 12 – 18             |
| Arabinose      | 8 – 14              |
| Glucose        | 6 – 10              |
| Fucose         | 2 – 5               |
| Mannose        | 1 – 3               |

The dominant xylose residue confirms the classification of flaxseed gum as an acidic arabinoxylan. The presence of rhamnose and uronic acid (Section 2) indicates co-extracted rhamnogalacturonan regions typical of mucilaginous seed polysaccharides. The xylose/arabinose ratio typically falls between 2.5 and 4.0.

---

## 4. Viscosity Properties

### 4.1 Apparent Viscosity vs. Concentration

Viscosity measured at 25 °C using a rotational rheometer (cone-and-plate geometry, shear rate = 10 s⁻¹, equilibration 120 s). Values are reported as a range across production lots.

| Concentration (% w/w) | Apparent Viscosity (cP) |
|------------------------|--------------------------|
| 0.1                    | 20 – 50                  |
| 0.5                    | 100 – 400                |
| 1.0                    | 500 – 2,000              |
| 2.0                    | 2,000 – 5,000            |
| 3.0                    | 5,000 – 10,000           |
| 5.0                    | 8,000 – 15,000           |

The gum exhibits a steep concentration-dependence typical of entangled polysaccharide solutions. At concentrations above 1 % (w/w), solutions form weak gels upon standing, though they remain shear-reversible.

### 4.2 Flow Behavior (Shear-Rate Sweep)

Shear-rate sweeps (0.1 – 1000 s⁻¹, 25 °C, 1 % w/w solution) are well-described by the Ostwald–de Waele power-law model:

**τ = K · γ̇ⁿ**

| Parameter | Value                      |
|-----------|----------------------------|
| n         | 0.30 – 0.50 (dimensionless)|
| K         | 5 – 50 Pa·sⁿ               |
| R²        | ≥ 0.99                     |

The flow index n < 1 confirms strong shear-thinning (pseudoplastic) behavior, enabling easy pumping, mixing, and filling while providing high low-shear viscosity for suspension and stabilization. At concentrations below 0.3 % the solution approaches Newtonian behavior (n → 1).

### 4.3 Thixotropy

A three-interval thixotropy test (low shear 0.1 s⁻¹ / high shear 500 s⁻¹ / low shear 0.1 s⁻¹) shows ≥ 85 % viscosity recovery within 120 s, indicating excellent structural regeneration.

---

## 5. Dynamic Oscillatory Rheology

### 5.1 Frequency Sweep

Oscillatory frequency sweeps are conducted from 0.01 to 10 Hz at 25 °C within the linear viscoelastic region (LVR, 1 % strain, determined by amplitude sweep).

| Frequency (Hz) | G' (Pa) — Typical | G'' (Pa) — Typical | tan δ |
|----------------|--------------------|--------------------|-------|
| 0.01           | 1.2 – 4.5          | 3.0 – 8.0          | 1.5–2.5 |
| 0.10           | 8.0 – 25           | 12 – 30            | 1.0–1.8 |
| 1.00           | 45 – 120           | 35 – 90            | 0.6–0.9 |
| 10.0           | 150 – 400          | 80 – 200           | 0.4–0.6 |

**Crossover frequency (G' = G''):** 0.05 – 0.30 Hz (1 % w/w, 25 °C).

Below the crossover, the gum solution exhibits liquid-like behavior (G'' > G'). Above the crossover, elastic behavior dominates (G' > G''), characteristic of an entangled polymer network with a characteristic relaxation time τ = 1/ω_c ≈ 3 – 20 s.

### 5.2 Temperature Sweep

Temperature ramps from 5 °C to 80 °C at 2 °C/min (1 % w/w, 1 Hz, 1 % strain, Peltier-controlled Peltier plate with solvent trap to prevent evaporation).

- **5 – 30 °C:** Apparent viscosity decreases by 35 – 50 % as hydrogen-bonding networks weaken.
- **30 – 60 °C:** Viscosity shows a plateau region with a mild slope (activation energy Eₐ ≈ 15 – 25 kJ/mol from Arrhenius fit).
- **60 – 80 °C:** Slight further decline; no thermal gelation or precipitous viscosity drop observed.
- **Cool-down (80 → 5 °C):** ≥ 90 % viscosity recovery, confirming thermal reversibility and absence of thermal degradation under these conditions.

The gum retains > 70 % of its room-temperature viscosity at 80 °C, indicating good thermal stability suitable for pasteurization and hot-fill processes.

### 5.3 Creep and Recovery

Creep/recovery tests: instantaneous application of constant stress τ₀ = 1 Pa (within LVR) for 300 s (creep), followed by stress removal and recovery monitored for 600 s (1 % w/w, 25 °C).

| Time (s) | Compliance J(t) (Pa⁻¹) — Typical |
|----------|----------------------------------|
| 1        | 0.002 – 0.015                    |
| 10       | 0.02 – 0.12                      |
| 100      | 0.15 – 0.60                      |
| 300      | 0.35 – 1.20                      |
| 600 (recovery) | 0.08 – 0.40 (residual compliance) |

**Burgers model parameters (four-element viscoelastic):**
- Instantaneous elastic compliance J₀: 0.002 – 0.010 Pa⁻¹
- Retarded compliance J₁: 0.10 – 0.40 Pa⁻¹
- Retardation time λᵣ: 15 – 50 s
- Zero-shear viscosity η₀: 80 – 300 Pa·s

Recovery efficiency ≥ 65 % (residual compliance after 600 s recovery relative to maximum creep compliance), demonstrating strong elastic recovery with minimal permanent deformation.

---

## 6. Critical Overlap Concentration

The critical overlap concentration c* marks the transition from the dilute to the semi-dilute entangled regime, determined from the intersection of the specific viscosity (ηₛₚ) vs. concentration double-log plot slopes.

| Parameter           | Specification   |
|---------------------|-----------------|
| c*                  | 0.3 – 0.5 % w/w |

At c > c*, individual polymer chains overlap and entangle, producing a sharp increase in zero-shear viscosity (η₀ ∝ c³·⁵). Below c*, η₀ scales as η₀ ∝ c¹·². The relatively low c* value reflects the high molecular weight (> 10⁶ Da) and extended conformation of flaxseed gum arabinoxylans in aqueous solution.

---

## 7. Emulsifying Properties

### 7.1 Emulsifying Activity Index (EAI)

Determined by turbidimetric method (spectrophotometry at 500 nm, oil-in-water emulsion, 0.5 % gum solution, soy oil/water 1:4, homogenized at 20,000 rpm, 1 min).

| Parameter | Specification |
|-----------|---------------|
| EAI       | 45 – 60 m²/g  |

### 7.2 Emulsion Stability Index (ESI)

| Parameter | Specification |
|-----------|---------------|
| ESI       | ≥ 85 %        |

EAI and ESI values confirm that flaxseed gum FSP-GUM-001 functions as an effective emulsifier, stabilizing oil droplets through a combination of steric repulsion (from the polysaccharide brush layer) and viscosity enhancement of the continuous phase. Performance is comparable to gum arabic and may be synergistic when blended.

---

## 8. Foaming Properties

### 8.1 Foam Overrun

| Parameter     | Specification    | Method                          |
|---------------|------------------|---------------------------------|
| Foam Overrun  | 100 – 150 %      | Whipping 1 % solution, 5 min, 25 °C |

### 8.2 Foam Stability

| Parameter      | Specification |
|----------------|---------------|
| Stability (2 h)| 70 – 85 %     |

Foam volume is maintained over 2 h owing to the high bulk viscosity and interfacial film elasticity imparted by the gum. The polysaccharide adsorbs at the air–water interface, retarding drainage and coalescence.

---

## 9. Emulsion Creaming Index

Creaming stability is assessed by gravity separation of an oil-in-water emulsion (10 % v/v soy oil, 0.5 % gum, stored quiescently at 25 °C in graduated cylinders).

| Time (h) | Creaming Index (%) — Typical |
|----------|-----------------------------|
| 0        | 0.0                         |
| 2        | 2 – 8                       |
| 6        | 5 – 15                      |
| 12       | 8 – 20                      |
| 24       | 10 – 25                     |

After 24 h, the creaming index remains ≤ 25 %, indicating a kinetically stable emulsion with no visible oil separation. The dense polysaccharide network retards droplet rise in accordance with Stokes' law.

---

## 10. Mineral and Heavy Metal Profile

| Element         | Specification Limit | Method         |
|-----------------|---------------------|----------------|
| Calcium (Ca)    | 800 – 2,500 mg/kg   | ICP-OES        |
| Potassium (K)   | 1,000 – 3,000 mg/kg | ICP-OES        |
| Magnesium (Mg)  | 400 – 1,200 mg/kg   | ICP-OES        |
| Sodium (Na)     | ≤ 500 mg/kg         | ICP-OES        |
| Iron (Fe)       | ≤ 50 mg/kg          | ICP-OES        |
| Zinc (Zn)       | ≤ 25 mg/kg          | ICP-OES        |
| Arsenic (As)    | ≤ 1.0 mg/kg         | ICP-MS         |
| Lead (Pb)       | ≤ 1.0 mg/kg         | ICP-MS         |
| Cadmium (Cd)    | ≤ 0.5 mg/kg         | ICP-MS         |
| Mercury (Hg)    | ≤ 0.1 mg/kg         | ICP-MS/AAS     |

All heavy metals comply with USP/NF, FCC, and EU food additive purity criteria (Commission Regulation (EU) No 231/2012).

---

## 11. Microbiological Specifications

| Test                          | Specification             | Method          |
|-------------------------------|---------------------------|-----------------|
| Total Plate Count (TVC)       | ≤ 1,000 CFU/g             | ISO 4833        |
| Yeast & Mold                  | ≤ 100 CFU/g               | ISO 21527       |
| Enterobacteriaceae            | ≤ 10 CFU/g                | ISO 21528       |
| _Escherichia coli_            | Negative in 10 g          | ISO 16649       |
| _Salmonella_ spp.             | Negative in 25 g          | ISO 6579        |
| _Staphylococcus aureus_       | Negative in 10 g          | ISO 6888        |
| _Bacillus cereus_             | ≤ 100 CFU/g               | ISO 7932        |
| _Listeria monocytogenes_      | Negative in 25 g          | ISO 11290       |
| Coliforms                     | ≤ 10 CFU/g                | ISO 4832        |
| Sulfite-Reducing Clostridia   | ≤ 10 CFU/g                | ISO 15213       |

The product undergoes terminal drying at inlet/outlet temperatures of 180 °C / 85 °C during spray-drying, which provides an additional microbiological kill step. The low water activity (a_w ≤ 0.35) inhibits post-process microbial growth.

---

## 12. Hygroscopicity — Moisture Sorption Isotherm

Moisture sorption is determined gravimetrically at 25 °C over a range of water activities (a_w = 0.10 – 0.90) using a dynamic vapor sorption (DVS) analyzer.

| Water Activity (a_w) | Equilibrium Moisture Content (% w/w) — Typical |
|-----------------------|-----------------------------------------------|
| 0.10                  | 3.0 – 4.5                                     |
| 0.20                  | 4.5 – 6.0                                     |
| 0.30                  | 6.0 – 8.0                                     |
| 0.40                  | 8.0 – 10.5                                    |
| 0.50                  | 10.5 – 13.0                                   |
| 0.60                  | 13.0 – 16.5                                   |
| 0.70                  | 16.5 – 21.0                                   |
| 0.80                  | 21.0 – 27.0                                   |
| 0.90                  | 28.0 – 35.0                                   |

The isotherm exhibits a Type II (S-shaped) BET profile, characteristic of hydrophilic polysaccharides. The monolayer moisture content (BET model) is 3.0 – 5.0 % w/w, corresponding to a_w ≈ 0.20 – 0.30. To prevent caking and loss of flowability, the product should be stored at a_w ≤ 0.50 (see Section 13).

---

## 13. Packaging

| Container Type          | Net Weight    | Material & Construction                                  |
|-------------------------|---------------|----------------------------------------------------------|
| Multi-wall Paper Bags   | 15 kg         | PE-lined kraft paper bags, heat-sealed inner liner       |
| Fibre Drums             | 200 kg        | PE-lined corrugated fibre drum with removable lid        |
| Bulk (IBC)              | 500 – 1,000 kg | Food-grade FIBC (flexible intermediate bulk container)   |

All packaging materials are food-grade, BPA-free, and compliant with EU Regulation 10/2011 and FDA 21 CFR 175.300. Each package is labelled with lot number, production date, expiry date, net weight, and storage instructions.

---

## 14. Storage and Shelf Life

| Condition                     | Recommendation                             |
|-------------------------------|--------------------------------------------|
| Temperature                   | ≤ 25 °C (controlled ambient)               |
| Relative Humidity             | ≤ 50 % RH                                  |
| Light Exposure                | Store in opaque or UV-protected packaging  |
| Shelf Life (sealed, as above) | 24 months from date of manufacture         |
| Shelf Life (after opening)    | 6 months (if resealed under same conditions)|

Under recommended conditions, the product retains ≥ 90 % of its initial viscosity (1 % solution, 10 s⁻¹) and passes all microbiological and heavy metal specifications at 24 months. Accelerated stability studies (40 °C, 75 % RH, 6 months) show no significant increase in moisture (> 6 %) or loss in EAI (< 10 % relative decline).

**Important storage notes:**
- Avoid temperature fluctuations exceeding 15 °C to prevent moisture migration and condensation inside the packaging.
- Do not stack pallets more than three units high to avoid compression damage to bags.
- Once opened, content should be used promptly and the container resealed tightly to minimize moisture uptake.

---

## 15. Regulatory Status and Applications

### 15.1 Regulatory

- **GRAS (USA):** Flaxseed gum may be used as a direct food ingredient under the generally recognized as safe provisions. A GRAS notification is on file with the FDA.
- **EU:** Not currently listed as an additive under Annex II of Regulation (EC) No 1333/2008; marketed as a food ingredient. Pending novel food authorization in certain member states.
- **China (GB 2760):** Accepted as a natural food additive for thickening and stabilizing in select categories.
- **Kosher / Halal:** Available upon request with third-party certification.

### 15.2 Typical Use Levels

| Application                     | Recommended Dosage (% w/w) |
|---------------------------------|----------------------------|
| Beverages (dairy & plant-based) | 0.05 – 0.30                |
| Sauces, Dressings, Gravies      | 0.20 – 0.80                |
| Baked Goods (gluten-free)       | 0.50 – 2.00                |
| Meat Products (binder)          | 0.30 – 1.00                |
| Ice Cream / Sorbet              | 0.10 – 0.40                |
| Edible Films & Coatings         | 0.50 – 3.00                |

---

## 16. Analytical Methods Reference Summary

| Property                | Method / Standard                                         |
|-------------------------|-----------------------------------------------------------|
| Total Polysaccharide    | Phenol-Sulfuric Acid (Dubois et al., 1956)                |
| Protein                 | AOAC 984.13 (Kjeldahl, N × 6.25)                          |
| Uronic Acid             | Blumenkrantz & Asboe-Hansen, 1973                          |
| Moisture                | AOAC 925.10                                                |
| Ash                     | AOAC 923.03                                                |
| Acetyl Groups           | HPLC (Reversed-Phase, UV 210 nm)                          |
| Monosaccharides         | HPLC-PAD after TFA hydrolysis                              |
| Viscosity               | Rotational Rheometer (cone/plate, 10 s⁻¹)                 |
| Oscillatory Rheology    | Stress-controlled rheometer, 25 °C, 1 % strain            |
| EAI / ESI               | Turbidimetric (Pearce & Kinsella, 1978)                   |
| Foaming                 | Whipping test (AACC Method 56-61.02)                      |
| Heavy Metals            | ICP-OES / ICP-MS                                           |
| Microbiology            | ISO methods per Section 11                                 |
| Moisture Sorption       | DVS (Dynamic Vapor Sorption) at 25 °C                     |

---

## 17. Revision History

| Version | Date       | Author         | Description of Change       |
|---------|------------|----------------|-----------------------------|
| 1.0     | 2026-07-20 | FlaxSeedsPro QA | Initial release             |

---

**END OF DOCUMENT**

*This specification is provided for informational and quality assurance purposes. Values represent typical production ranges under controlled conditions. Actual lot-specific certificates of analysis (COA) are available upon request. Contact FlaxSeedsPro Technical Services for further information or custom specification inquiries.*
