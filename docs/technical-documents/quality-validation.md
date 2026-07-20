# Quality Validation & QC Systems

## 1. Method Validation — Parameters and Protocol

All analytical test methods used for raw material, in-process, and finished product release are validated according to **ICH Q2(R1)** and **AOAC International** guidelines. The following parameters are evaluated for each method during initial validation and subsequent re-validation (triggered by method changes, instrument changes, or at intervals not exceeding 3 years).

### 1.1 Validation Parameters

| Parameter | Definition | Acceptance Criterion |
|-----------|-----------|---------------------|
| **Accuracy (Trueness)** | Closeness of agreement between measured value and true/reference value, expressed as % recovery | 98–102% (or as specified per method) |
| **Precision (Repeatability)** | Agreement among replicate measurements under same conditions (same operator, instrument, day) | RSD ≤ 2% (or as specified) |
| **Intermediate Precision (Reproducibility)** | Agreement among replicates across operators, instruments, and days | RSD ≤ 3% (or as specified) |
| **Limit of Detection (LOD)** | Lowest concentration that can be reliably detected (S/N ≥ 3:1 or 3σ of blank) | ≤ 1/10 of specification limit |
| **Limit of Quantification (LOQ)** | Lowest concentration that can be quantified with acceptable accuracy and precision (S/N ≥ 10:1 or 10σ of blank) | ≤ 1/5 of specification limit |
| **Linearity** | Ability to obtain test results proportional to concentration over a defined range | \( r^2 \geq 0.995 \) |
| **Range** | Interval between upper and lower concentrations with demonstrated precision, accuracy, and linearity | Covers 50–150% of expected specification range |
| **Robustness** | Capacity to remain unaffected by small, deliberate variations in method parameters | RSD ≤ 2% across varied conditions |
| **Selectivity / Specificity** | Ability to measure analyte unequivocally in presence of matrix components | No interference > LOD at retention time |
| **Uncertainty** | Combined standard uncertainty from all validated sources | See Section 6 |

### 1.2 Validation Protocol Requirements

Each validation study follows a pre-approved validation protocol that specifies:
- Number of replicates (minimum 10 for precision, minimum 3 concentration levels × 3 replicates for accuracy)
- Reference materials (certified reference material [CRM] or in-house reference standard with traceable assignment)
- Statistical treatment (ANOVA for precision components, linear regression for linearity, Student's t-test for bias)
- Acceptance criteria (pre-defined before study initiation)
- Outlier handling (Grubbs' test, α = 0.05)

## 2. Validation Data for Key Analytical Methods

### 2.1 Moisture Content — Air Oven Method (AOCS Ba 2a-38)

| Parameter | Result | Acceptance Criterion | Status |
|-----------|--------|---------------------|--------|
| Repeatability (SD) | **0.10%** | ≤ 0.15% | ✅ Pass |
| Repeatability (RSD) | **1.1%** (at 8.5% moisture) | ≤ 2.0% | ✅ Pass |
| Intermediate precision (SD) | **0.12%** | ≤ 0.20% | ✅ Pass |
| Accuracy (% recovery on CRM) | **99.7%** | 98.0–102.0% | ✅ Pass |
| LOD | **0.03%** | — | ✅ Acceptable |
| LOQ | **0.10%** | — | ✅ Acceptable |
| Linearity (\( r^2 \)) | **0.998** | ≥ 0.995 | ✅ Pass |
| Range | 0.1–20.0% H₂O | 1.0–15.0% (required) | ✅ Pass |

### 2.2 Protein Content — Dumas Combustion (AOCS Ba 4e-93 / AOAC 990.03)

| Parameter | Result | Acceptance Criterion | Status |
|-----------|--------|---------------------|--------|
| Repeatability (RSD) | **1.8%** (at 36% protein d.b.) | ≤ 2.0% | ✅ Pass |
| Intermediate precision (RSD) | **2.2%** | ≤ 3.0% | ✅ Pass |
| Accuracy (% recovery on CRM) | **100.3%** | 98.0–102.0% | ✅ Pass |
| LOD | **0.05% N** (0.31% protein) | — | ✅ Acceptable |
| LOQ | **0.10% N** (0.63% protein) | — | ✅ Acceptable |
| Linearity (\( r^2 \)) | **0.9996** | ≥ 0.995 | ✅ Pass |
| Range | 0.63–60.0% protein | 5.0–50.0% (required) | ✅ Pass |

### 2.3 Alpha-Linolenic Acid (ALA) by GC-FID (AOCS Ce 1h-05)

| Parameter | Result | Acceptance Criterion | Status |
|-----------|--------|---------------------|--------|
| Repeatability (RSD) | **1.4%** (at 52% ALA of total FA) | ≤ 1.5% | ✅ Pass |
| Intermediate precision (RSD) | **1.7%** | ≤ 2.5% | ✅ Pass |
| Accuracy (% recovery on CRM) | **100.1%** | 98.0–102.0% | ✅ Pass |
| LOD | **0.02%** of total FAME | — | ✅ Acceptable |
| LOQ | **0.06%** of total FAME | — | ✅ Acceptable |
| Linearity (\( r^2 \)) | **0.999** | ≥ 0.995 | ✅ Pass |
| Range | 0.06–70.0% ALA | 10.0–65.0% (required) | ✅ Pass |

### 2.4 Free Fatty Acids (FFA) — Titration (AOCS Ca 5a-40)

| Parameter | Result | Acceptance Criterion | Status |
|-----------|--------|---------------------|--------|
| Repeatability (RSD) | **1.6%** (at 1.5% FFA as oleic) | ≤ 2.0% | ✅ Pass |
| Intermediate precision (RSD) | **2.0%** | ≤ 3.0% | ✅ Pass |
| Accuracy (% recovery) | **99.5%** | 98.0–102.0% | ✅ Pass |
| LOD | **0.02%** FFA | — | ✅ Acceptable |
| LOQ | **0.05%** FFA | — | ✅ Acceptable |
| Linearity (\( r^2 \)) | **0.997** | ≥ 0.995 | ✅ Pass |
| Range | 0.05–10.0% FFA | 0.1–5.0% (required) | ✅ Pass |

### 2.5 Peroxide Value (PV) — Titration (AOCS Cd 8b-90)

| Parameter | Result | Acceptance Criterion | Status |
|-----------|--------|---------------------|--------|
| Repeatability (RSD) | **2.5%** (at 2.0 meq/kg) | ≤ 3.0% | ✅ Pass |
| Intermediate precision (RSD) | **3.1%** | ≤ 4.0% | ✅ Pass |
| Accuracy (% recovery) | **99.2%** | 97.0–103.0% | ✅ Pass |
| LOD | **0.05 meq/kg** | — | ✅ Acceptable |
| LOQ | **0.15 meq/kg** | — | ✅ Acceptable |
| Linearity (\( r^2 \)) | **0.996** | ≥ 0.995 | ✅ Pass |
| Range | 0.15–25.0 meq/kg | 0.2–15.0 (required) | ✅ Pass |

## 3. Control Charts for Routine QC

### 3.1 X-bar and R Chart Implementation

All routine QC parameters are monitored using **Shewhart X-bar and R control charts** as per ASTM E2587 and ISO 7870-2. Charts are maintained in the LIMS (LabWare v8) with automated data entry from analytical instruments.

### 3.2 Parameters and Sampling Frequency

| Parameter | Product | Frequency | Subgroup Size (n) | Chart Period |
|-----------|---------|-----------|-------------------|--------------|
| Moisture (%) | Meal | 1 per production shift | 5 replicate readings | Rolling 25 subgroups |
| Protein (% d.b.) | Meal | 1 per production shift | 5 replicate readings | Rolling 25 subgroups |
| ALA (% of total FA) | Oil | 1 per batch | 3 replicate injections | Rolling 25 subgroups |
| FFA (%) | Oil (crude) | 1 per batch | 3 replicates | Rolling 25 subgroups |
| FFA (%) | Oil (refined) | 1 per batch | 3 replicates | Rolling 25 subgroups |
| Peroxide value (meq/kg) | Oil (RBD) | 1 per batch | 3 replicates | Rolling 25 subgroups |
| Color (Lovibond, red) | Oil (RBD) | 1 per batch | 3 replicates | Rolling 25 subgroups |

### 3.3 Control Limits

Control limits are calculated from **20 initial subgroups** (minimum 100 individual readings) and reviewed quarterly. Limits are updated when justified by process improvement or when 25 new subgroups demonstrate a sustained shift.

- **Warning Limits** (Upper/Lower): mean ± 2σ (plotted as dashed lines)
- **Action Limits** (Upper/Lower): mean ± 3σ (plotted as solid red lines)
- **Range Limits** (Upper): \( D_4 \times \bar{R} \)

### 3.4 Out-of-Control Rules (Western Electric Rules)

The following rules trigger investigation and corrective action:

| Rule | Description | Action |
|------|-------------|--------|
| Rule 1 | Any point beyond ±3σ (action limit) | Immediate hold, root cause investigation |
| Rule 2 | 2 of 3 consecutive points beyond ±2σ (on same side) | Alert, increased monitoring frequency |
| Rule 3 | 4 of 5 consecutive points beyond ±1σ (on same side) | Alert, investigate assignable cause |
| Rule 4 | 8 consecutive points on same side of center line | Alert, evaluate for process bias adjustment |
| Rule 5 | 6 consecutive points trending up or down | Alert, check instrument drift |
| Rule 6 | Any point beyond UCL on R chart | Increase in variability, instrument/operator check |
| Rule 7 | 14 consecutive points alternating up/down | Possible over-control or sampling issue |

### 3.5 Example — Moisture Control Chart (Meal)

Current operating state (last 25 subgroups, n=5, data from Q2 2026):

| Parameter | Value |
|-----------|-------|
| Grand mean (\(\bar{\bar{x}}\)) | 8.52% |
| UCL (\(\bar{x}\)) | 8.92% |
| LCL (\(\bar{x}\)) | 8.12% |
| UWL (\(\bar{x}\)) | 8.78% |
| LWL (\(\bar{x}\)) | 8.26% |
| Mean range (\(\bar{R}\)) | 0.28% |
| UCL (\(R\)) | 0.62% |
| Process capability (Cpk) | 1.53 |

## 4. Proficiency Testing

### 4.1 Program Overview

The laboratory participates in external proficiency testing (PT) schemes to demonstrate technical competence and comply with **ISO/IEC 17025** requirements. Successful participation is mandatory for method accreditation maintenance.

### 4.2 Participation Schedule

| Analysis Type | Scheme Provider | Frequency | Samples per Round | Accredited Since |
|--------------|----------------|-----------|-------------------|------------------|
| Food microbiology (APC, Coliforms, E. coli, Salmonella, Yeast/Mold) | FAPAS (Fera Science) | **2× per year** (Apr, Oct) | 2 per round | 2018 |
| Oilseed chemistry (moisture, protein, oil, fiber) | AOCS Laboratory Proficiency Program | **1× per year** (September) | 2 per round | 2019 |
| Fatty acid profile (GC-FID) | AOCS Laboratory Proficiency Program | **1× per year** (March) | 2 per round | 2019 |
| Oil quality (FFA, PV, color, anisidine value) | LGC Standards (QCS) | **1× per year** (June) | 2 per round | 2020 |
| Trace metals (ICP-MS) | FAPAS | **1× per year** (November) | 2 per round | 2021 |
| Mycotoxins (aflatoxins, DON, OTA) | FAPAS | **1× per year** (August) | 2 per round | 2021 |

### 4.3 Performance Evaluation

Performance is assessed using the **z-score**:

\[
z = \frac{(x_i - x_a)}{\sigma_p}
\]

where \( x_i \) = reported result, \( x_a \) = assigned value, \( \sigma_p \) = standard deviation for proficiency assessment.

| z-score | Rating | Action |
|---------|--------|--------|
| \|z\| ≤ 2.0 | Satisfactory | None required |
| 2.0 < \|z\| < 3.0 | Warning (Questionable) | Investigate, document root cause |
| \|z\| ≥ 3.0 | Unsatisfactory | Mandatory root cause analysis, corrective action, re-testing within 30 days |

### 4.4 Historical Performance

Over the past 5 years (2021–2026):
- **98.2%** of results rated Satisfactory (|z| ≤ 2.0)
- **1.5%** rated Questionable (2.0 < |z| < 3.0) — all resolved with corrective action
- **0.3%** rated Unsatisfactory (|z| ≥ 3.0) — 2 events (one pH meter calibration drift in 2022, one FFA titration endpoint detection issue in 2023), both closed with CAPA

## 5. Inter-Laboratory Comparison

### 5.1 Annual Round Robin Protocol

An inter-laboratory comparison (round robin) is conducted **annually** in November with our partner laboratory (Eurofins Scientific, Hamburg, Germany). The protocol follows ISO 5725-2.

### 5.2 Scope and Samples

| Parameter | Material | Expected Range | Lab 1 (Internal) Method | Lab 2 (Partner) Method |
|-----------|----------|---------------|------------------------|------------------------|
| Moisture | Flaxseed meal | 7–10% | AOCS Ba 2a-38 | ISO 665:2020 |
| Protein (N×6.25) | Flaxseed meal | 32–38% d.b. | AOCS Ba 4e-93 | ISO 16634:2016 |
| Oil content | Flaxseed | 38–44% | AOCS Am 2-93 | ISO 659:2009 |
| ALA (C18:3n-3) | Flaxseed oil | 48–58% of FA | AOCS Ce 1h-05 | AOCS Ce 1i-07 |
| FFA | Crude flax oil | 0.5–3.0% | AOCS Ca 5a-40 | AOCS Ca 5a-40 |
| Peroxide value | Refined oil | 0–5 meq/kg | AOCS Cd 8b-90 | ISO 3960:2017 |

### 5.3 Evaluation Criteria

| Metric | Acceptance Criterion |
|--------|---------------------|
| Reproducibility SD (S_R) | ≤ 1.5× Horwitz SD (for composition) or ≤ 2× method precision (for oil quality) |
| HorRat value | 0.3 ≤ HorRat ≤ 1.5 |
| Bias between labs | Not statistically significant at α = 0.05 (paired t-test) |
| Relative bias | ≤ 3% for major components (> 10% concentration), ≤ 10% for trace components |

### 5.4 2025 Round Robin Results (Selected Parameters)

| Parameter | Internal Lab Mean | Partner Lab Mean | Bias | HorRat | Status |
|-----------|------------------|------------------|------|--------|--------|
| Moisture (%) | 8.51 | 8.47 | +0.04 | 0.42 | ✅ Pass |
| Protein (% d.b.) | 35.8 | 35.5 | +0.3 | 0.51 | ✅ Pass |
| ALA (% of FA) | 52.3 | 52.0 | +0.3 | 0.38 | ✅ Pass |
| FFA (%) | 1.18 | 1.21 | −0.03 | 0.55 | ✅ Pass |
| PV (meq/kg) | 0.92 | 0.88 | +0.04 | 0.61 | ✅ Pass |

## 6. Uncertainty Budget

### 6.1 Methodology

Measurement uncertainty is estimated following the **GUM** (Guide to the Expression of Uncertainty in Measurement, JCGM 100:2008) bottom-up approach. Combined standard uncertainty (\( u_c \)) is calculated by propagating individual uncertainty components, and expanded uncertainty (\( U \)) is reported using a coverage factor of \( k = 2 \) (95% confidence level).

### 6.2 Uncertainty Components

For each method, the following sources are quantified:

- **Sampling** (\( u_{\text{samp}} \)): Sub-sampling variability from replicate sample preparations
- **Weighing** (\( u_{\text{wt}} \)): Balance calibration and linearity
- **Volumetric** (\( u_{\text{vol}} \)): Pipette/volumetric flask calibration, temperature effects
- **Instrument** (\( u_{\text{inst}} \)): Calibration curve fitting residuals, detector linearity, drift
- **Repeatability** (\( u_{\text{rep}} \)): Within-run standard deviation from validation data
- **Reproducibility** (\( u_{\text{repr}} \)): Between-run standard deviation from intermediate precision
- **Reference material** (\( u_{\text{CRM}} \)): Uncertainty of certified value of CRM
- **Bias** (\( u_{\text{bias}} \)): Standard uncertainty of mean recovery from CRM analysis

### 6.3 Uncertainty Budgets — Key Parameters

#### Moisture (Air Oven) — Flaxseed Meal

| Component | Source | Value | Distribution | \( u_i \) |
|-----------|--------|-------|-------------|-----------|
| Weighing | Balance (0.1 mg) | ±0.0001 g | Rectangular | 0.00006 g |
| Sampling | Sub-sample variation | SD = 0.036% | Normal | 0.036% |
| Repeatability | Validation data | SD = 0.10% | Normal | 0.100% |
| Intermediate precision | Validation data | SD = 0.12% | Normal | 0.120% |
| Bias | CRM recovery (99.7%) | 0.3% bias | Rectangular | 0.173% |
| **Combined (\( u_c \))** | | | | **0.238%** |
| **Expanded (\( U \), \( k=2 \))** | | | | **0.48%** |

#### Protein (Dumas Combustion) — Flaxseed Meal

| Component | Source | Value | Distribution | \( u_i \) |
|-----------|--------|-------|-------------|-----------|
| Repeatability | Validation RSD = 1.8% at 36% | SD = 0.648% | Normal | 0.648% |
| Intermediate precision | Validation RSD = 2.2% | SD = 0.792% | Normal | 0.792% |
| Bias | CRM recovery (100.3%) | 0.3% bias | Rectangular | 0.173% |
| Conversion factor (N×6.25) | Literature uncertainty | ±0.02 | Rectangular | 0.19% (rel) |
| **Combined (\( u_c \))** | | | | **1.03%** |
| **Expanded (\( U \), \( k=2 \))** | | | | **2.06%** |

#### ALA by GC-FID — Flaxseed Oil

| Component | Source | Value | Distribution | \( u_i \) |
|-----------|--------|-------|-------------|-----------|
| Repeatability | Validation RSD = 1.4% at 52% | SD = 0.728% | Normal | 0.728% |
| Intermediate precision | Validation RSD = 1.7% | SD = 0.884% | Normal | 0.884% |
| Calibration curve | Linear regression residual | SD = 0.42% | Normal | 0.420% |
| FAME preparation | Transesterification yield | ±0.5% | Rectangular | 0.289% |
| Bias | CRM recovery (100.1%) | 0.1% bias | Rectangular | 0.058% |
| **Combined (\( u_c \))** | | | | **1.27%** |
| **Expanded (\( U \), \( k=2 \))** | | | | **2.54%** |

#### Free Fatty Acids (Titration) — Crude Oil

| Component | Source | Value | Distribution | \( u_i \) |
|-----------|--------|-------|-------------|-----------|
| Repeatability | Validation RSD = 1.6% at 1.5% | SD = 0.024% | Normal | 0.024% |
| Intermediate precision | Validation RSD = 2.0% | SD = 0.030% | Normal | 0.030% |
| Titrant concentration | Standardization (4 determinations) | SD = 0.0002 N | Normal | 0.001% |
| Titrant volume | Burette calibration (±0.02 mL) | 0.02 mL | Rectangular | 0.012% |
| Endpoint detection | Indicator color change | ±0.01 mL | Rectangular | 0.006% |
| **Combined (\( u_c \))** | | | | **0.042%** |
| **Expanded (\( U \), \( k=2 \))** | | | | **0.084%** |

#### Peroxide Value (Titration) — Refined Oil

| Component | Source | Value | Distribution | \( u_i \) |
|-----------|--------|-------|-------------|-----------|
| Repeatability | Validation RSD = 2.5% at 2.0 meq/kg | SD = 0.050 meq/kg | Normal | 0.050 |
| Intermediate precision | Validation RSD = 3.1% | SD = 0.062 meq/kg | Normal | 0.062 |
| Sample mass | Balance (±0.01 g) | 0.01 g | Rectangular | 0.006 meq/kg |
| Thiosulfate conc. | Standardization | SD = 0.0003 N | Normal | 0.008 meq/kg |
| Blank correction | Blank titration | SD = 0.01 mL | Normal | 0.005 meq/kg |
| **Combined (\( u_c \))** | | | | **0.081 meq/kg** |
| **Expanded (\( U \), \( k=2 \))** | | | | **0.16 meq/kg** |

## 7. Shelf Life Validation Protocol

### 7.1 Scope

Shelf life validation is conducted for all finished product SKUs prior to initial market release and subsequently at intervals not exceeding 5 years, or whenever there is a significant change in formulation, processing, or packaging.

### 7.2 Protocols by Storage Condition

| Condition | Temperature | RH | Light | Duration | Sampling Intervals |
|-----------|-------------|----|-------|----------|-------------------|
| **Real-time Ambient** | 25 ± 2 °C | 60 ± 5% RH | Dark (cardboard outer + opaque inner) | Target shelf life + 20% (e.g., 15 months for 12-month target) | T₀, 1, 2, 3, 6, 9, 12, 15 months |
| **Real-time Refrigerated** | 4 ± 2 °C | Ambient | Dark | Target shelf life + 30% | T₀, 3, 6, 9, 12, 18, 24 months |
| **Accelerated 1 (moderate)** | 40 ± 2 °C | 75 ± 5% RH | Dark | 6 months (correlation factor ≈ 2.5× to ambient) | T₀, 1, 2, 3, 4, 6 months |
| **Accelerated 2 (elevated)** | 50 ± 2 °C | Ambient | Dark | 3 months (screening only, not used for shelf life claim) | T₀, 1, 2, 3 months |
| **Light stress** | 25 ± 2 °C | 60 ± 5% RH | 1200 lux cool-white fluorescent, 12 h on/off cycle | 3 months | T₀, 1 week, 2 weeks, 1, 2, 3 months |

### 7.3 Kinetic Modeling

For accelerated conditions, the **Arrhenius model** is used to estimate reaction rate acceleration factors:

\[
k = A \cdot e^{-E_a / (RT)}
\]

Where:
- \( k \) = reaction rate constant
- \( E_a \) = activation energy (kJ/mol), estimated from triplicate temperature points
- \( R \) = universal gas constant (8.314 J/mol·K)
- \( T \) = absolute temperature (K)

The **Q₁₀** factor (fold-change in rate per 10 °C increase) is calculated for each stability-indicating parameter. A Q₁₀ value between 2.0 and 3.0 is considered typical for lipid oxidation reactions.

### 7.4 Acceptance Criteria for Shelf Life

The end of shelf life is defined as the time point at which any measured parameter exceeds the following limits:

| Parameter | Flaxseed Crude Oil | Flaxseed RBD Oil | Flaxseed Meal |
|-----------|-------------------|------------------|---------------|
| FFA (% as oleic) | ≤ 3.0% | ≤ 0.5% | — |
| Peroxide value (meq/kg) | ≤ 10.0 | ≤ 5.0 | — |
| p-Anisidine value | ≤ 20.0 | ≤ 10.0 | — |
| ALA (% of total FA) | ≥ 48.0% (or ≥ 90% of T₀ value) | ≥ 48.0% (or ≥ 90% of T₀ value) | — |
| Moisture | — | — | ≤ 10.0% |
| Color (Lovibond red, 5¼\" cell) | ≤ 15.0 | ≤ 3.0 | — |
| Free-flowing (visual) | — | — | No clumps > 2 cm |
| Aerobic plate count (CFU/g) | ≤ 10,000 | ≤ 1,000 | ≤ 100,000 |
| Yeast & Mold (CFU/g) | ≤ 100 | ≤ 10 | ≤ 1,000 |
| Sensory (odor, taste) | No rancid off-notes (trained panel, n ≥ 3) | No rancid off-notes | No musty or sour odor |

### 7.5 Statistical Analysis

- Shelf life is estimated by **linear regression** of each parameter vs. time (with 95% confidence bands)
- The lower one-sided 95% confidence limit is used to determine the time at which the parameter crosses the specification limit
- The **minimum** of all calculated shelf lives across all parameters is declared as the product shelf life
- For accelerated studies, the shelf life estimate is validated against the real-time study at the 12-month time point

## 8. Stability-Indicating Parameters by Product

### 8.1 Flaxseed Crude Oil (FLO-01)

| Parameter | Primary or Secondary Indicator | Rationale |
|-----------|-------------------------------|-----------|
| FFA | **Primary** | Direct measure of hydrolytic rancidity; increases with moisture and enzymatic activity |
| Peroxide value | **Primary** | Primary oxidation product (hydroperoxides); most sensitive early indicator |
| p-Anisidine value | **Primary** | Secondary oxidation products (aldehydes); indicates advanced oxidation |
| ALA content | **Primary** | Omega-3 is the key nutritional claim; loss via oxidation must be quantified |
| Color (Lovibond red) | Secondary | Browning due to non-enzymatic reactions |
| Tocopherol content | Secondary | Natural antioxidant depletion correlates with oxidation progression |
| Sensory (odor) | **Primary** | Consumer-facing attribute; rancid notes correlate with chemical markers |

### 8.2 Flaxseed RBD Oil (FLO-02)

| Parameter | Primary or Secondary Indicator | Rationale |
|-----------|-------------------------------|-----------|
| Peroxide value | **Primary** | Most sensitive oxidation marker in refined oil (low initial PV) |
| p-Anisidine value | **Primary** | Total oxidation (TOTOX = 2×PV + AnV) provides combined oxidation status |
| FFA | **Primary** | Low initial FFA (< 0.1%); any increase indicates improper refining or hydrolysis |
| ALA content | **Primary** | Nutritional claim integrity; omega-3 retention is critical |
| Color (Lovibond red) | Secondary | Color reversion indicates oxidation or bleaching effectiveness |
| Sensory (odor, taste) | **Primary** | Refined oil must remain bland; any off-flavor is a defect |
| Rancimat induction time | Secondary | Accelerated stability screening tool |

### 8.3 Flaxseed Meal (FOM-01)

| Parameter | Primary or Secondary Indicator | Rationale |
|-----------|-------------------------------|-----------|
| Moisture | **Primary** | Drives microbial growth and caking; critical for storage stability |
| Water activity (aw) | **Primary** | < 0.60 aw prevents microbial proliferation |
| Aerobic plate count | **Primary** | Indicator of microbial stability and hygiene |
| Yeast & Mold | **Primary** | Specific spoilage organisms for oilseed meals |
| Free-flowing characteristic | **Primary** | Functional attribute; caking indicates moisture migration |
| Color (Hunter L, a, b) | Secondary | Browning indicates Maillard reactions during storage |
| Protein solubility | Secondary | Indicator of heat damage during storage (less critical for meal vs. protein concentrate) |
| Peroxide value | Secondary | Residual oil in meal (8–12%) can oxidize; meal PV correlates with off-odors |

### 8.4 Testing Frequency During Shelf Life

| Time Point | Full QC Panel (all stability parameters) | Reduced Panel (primary indicators only) |
|------------|------------------------------------------|----------------------------------------|
| T₀ (baseline, 1 week after production) | ✅ | — |
| 1 month | — | ✅ |
| 2 months | — | ✅ |
| 3 months | ✅ | — |
| 6 months | ✅ | — |
| 9 months | — | ✅ |
| 12 months | ✅ | — |
| 15 months (if applicable) | ✅ | — |

---

*Document reference: QVAL-001 Rev 2.4*
*Last reviewed: 2026-06-20*
*Next review: 2027-06-20*
