# Gum Extraction & Purification Line — Equipment Specification

## 1. Process Objective

Extract, purify, and dry soluble polysaccharide gum (flaxseed mucilage) from whole or crushed flaxseed to produce a food-grade gum powder with viscosity ≥ 800 cP (1 % solution, 25 °C). The line operates at a throughput of **200 kg/hr** dried gum powder. This station is designated **CCP-3** (Critical Control Point — Residual Solvent & Allergen Control).

---

## 2. Equipment Configuration & Flow Diagram

```
Flaxseed (whole or light-crushed)
    │
    ▼
[ Extraction Tank (Jacketed, 2000 L) ]  ← Hot water (80–90 °C, pH 6–7)
    │
    ▼
[ Decanter Centrifuge ] ───→ Wet solids (spent seed, to drying/meal)
    │
    ▼
[ Vacuum Concentrator ] ───→ Concentrated gum liquor (5–8 % solids)
    │
    ▼
[ Precipitation Tank ]  ← Ethanol (96 % v/v, 2:1 vol ratio)
    │
    ▼
[ Basket Centrifuge ] ───→ Spent ethanol (to recovery)
    │
    ▼
Wet gum cake (≈ 60 % moisture)
    │
    ▼
[ Spray Dryer ] ───→ Dried gum powder (≤ 6 % moisture)
    │                       │
    ▼                       ▼
[ Ethanol Recovery Column ]     [ Sifter / Pack-off ]
    │
    ▼
Recovered ethanol (≥ 90 % v/v, recycled to precipitation)
```

---

## 3. Equipment Specifications

### 3.1 Gum Extraction Tank
| Parameter             | Value                             |
|-----------------------|-----------------------------------|
| Type                  | Jacketed, agitated, atmospheric   |
| Working volume         | 2 000 L                          |
| Material               | **SS316** (all wetted parts)      |
| Jacket                 | Half-coil, rated 4 bar(g) steam   |
| Agitator               | Dual impeller (hydrofoil + Rushton)|
| Agitator speed         | 50 – 200 rpm (VFD)               |
| Motor                  | 7.5 kW, IE3, TEFC                |
| Temp. range            | Ambient – 100 °C (target 85 °C)  |
| pH range               | 3 – 8 (target pH 6.0 – 6.5)     |
| Batch cycle            | 45 – 60 min extraction           |
| Water-to-seed ratio    | 10:1 – 15:1 (w/w)               |
| Inspection             | 2 × 150 mm manway, sight glass   |
| CIP                    | Fixed spray ball (SS316)         |

### 3.2 Decanter Centrifuge
| Parameter             | Value                             |
|-----------------------|-----------------------------------|
| Type                  | Horizontal solid-bowl decanter    |
| Bowl diameter         | 350 mm                            |
| Bowl length / diameter| 3.5 : 1                           |
| Max G-force           | 3 500 × g                         |
| Differential speed    | 5 – 20 rpm (VFD on scroll)        |
| Capacity (slurry)     | 3 000 L/hr                        |
| Solids capture        | ≥ 95 % of suspended solids        |
| Material              | SS316 bowl, SS316L scroll         |
| Motor (bowl)          | 15 kW                             |
| Motor (scroll)        | 5.5 kW                            |
| Discharge             | Solids: gravity chute; Liquid: gravity overflow|

### 3.3 Vacuum Concentrator
| Parameter             | Value                             |
|-----------------------|-----------------------------------|
| Type                  | Forced-circulation evaporator     |
| Evaporation rate      | 500 kg/hr (water removal)         |
| Vacuum level          | −0.80 to −0.92 bar(g)             |
| Temp. (product)       | ≤ 65 °C (protect gum viscosity)  |
| Heating surface       | 15 m² (SS316 plate heat exchanger)|
| Vapour separator      | Cyclone + mesh pad (SS316)        |
| Motor (circulation)   | 7.5 kW                            |
| Material              | SS316 (all wetted surfaces)       |
| Feed solids in        | 0.8 – 1.5 %                       |
| Concentrate solids out| 5 – 8 % (20× concentration)       |
| Condenser             | Shell-and-tube, SS316, 25 m²      |
| Cooling water         | 15 m³/hr @ 25 °C                 |

### 3.4 Precipitation Tank
| Parameter             | Value                             |
|-----------------------|-----------------------------------|
| Type                  | Flat-bottom, agitated             |
| Working volume         | 3 000 L                           |
| Material               | SS316                             |
| Agitator               | Paddle (low shear)                |
| Speed                  | 30 – 60 rpm                       |
| Motor                  | 3 kW                              |
| Ethanol feed           | Sub-surface dip pipe              |
| Ratio control          | In-line flowmeter + batch PLC     |

### 3.5 Basket Centrifuge
| Parameter             | Value                             |
|-----------------------|-----------------------------------|
| Type                  | Vertical peeler / basket          |
| Basket diameter       | 800 mm                            |
| Basket volume         | 100 L                             |
| Max G-force           | 1 200 × g                         |
| Filter media          | Polypropylene cloth (20–50 µm)    |
| Cycle time            | 15 – 25 min (fill → spin → peel)  |
| Capacity (wet cake)   | 100 kg/batch                      |
| Material              | SS316 basket, SS304 housing       |
| Motor                 | 11 kW (VFD soft-start)            |
| Explosion-proof       | **Ex d IIB T4** (ethanol atmosphere)|

### 3.6 Spray Dryer
| Parameter             | Value                             |
|-----------------------|-----------------------------------|
| Type                  | Co-current, centrifugal atomiser  |
| Evaporation rate      | 200 kg/hr (water)                 |
| Inlet air temperature | **180 °C** (max 200 °C)           |
| Outlet air temperature| **80 °C** (range 75–85 °C)        |
| Atomiser wheel        | Disk type, 15 000 – 25 000 rpm    |
| Atomiser motor        | 5.5 kW, VFD                       |
| Drying chamber        | SS316, Ø 2 200 mm, cylindrical    |
| Cyclone               | SS316, ≥ 98 % collection          |
| Bag filter            | SS316 housing, PTFE membrane bags |
| Product outlet        | Powder at ≤ 60 °C                 |
| Final moisture        | ≤ 6 % (target 4–5 %)             |
| Throughput (powder)   | **≈ 200 kg/hr**                   |
| CIP                   | Fixed spray ball in chamber       |
| Ex-proof              | Outlet rated for combustible dust (ATEX Zone 22)|

### 3.7 Sifter / Classifier
| Parameter             | Value                             |
|-----------------------|-----------------------------------|
| Type                  | Gyratory / tumbler screen         |
| Mesh                  | 250 µm (60 mesh)                  |
| Capacity              | 250 kg/hr                         |
| Material              | SS316 contact                     |

### 3.8 Ethanol Recovery Column
| Parameter             | Value                             |
|-----------------------|-----------------------------------|
| Type                  | Packed column (Raschig rings / Pall rings)|
| Column diameter       | DN 300                             |
| Packed height         | 4 000 mm                           |
| Distillate rate       | **50 L/hr** (≈ 90 % v/v ethanol)  |
| Feed (spent ethanol)  | 40 – 60 % v/v ethanol             |
| Reboiler              | Thermosiphon, SS316, 12 m²         |
| Condenser             | Shell-and-tube, SS316, 10 m²       |
| Reflux ratio          | 2:1 – 4:1 (PID controlled)        |
| Column ΔP             | ≤ 50 mbar                          |
| Material              | SS316 column + internals           |
| Automation            | Temp. profile (top/bottom) → reflux control valve|

---

## 4. Process & Performance Targets

| Metric                          | Target                    | Monitoring Method              |
|---------------------------------|---------------------------|--------------------------------|
| Gum extraction yield            | ≥ 85 % of available gum   | Mass balance (seed vs powder)  |
| Gum purity (as polysaccharide)  | ≥ 75 % (w/w)              | AOAC 991.43 (TDF)              |
| Viscosity (1 % sol., 25 °C)    | ≥ 800 cP                  | Brookfield LVDV (spindle #3)   |
| Residual ethanol in powder      | **≤ 50 ppm** (CCP-3)      | GC-HS (per batch)              |
| Moisture content (powder)       | ≤ 6 %                     | Halogen analyser (105 °C)      |
| Particle size (D90)             | ≤ 250 µm                  | Sieve analysis / laser diff.   |
| Ethanol recovery efficiency     | ≥ 95 %                    | Mass balance (in vs recovered) |
| Spray dryer outlet temp (CCP-3)| **75–85 °C**              | In-line RTD (interlocked on T-out)|

---

## 5. HACCP — CCP-3 Integration

| CCP | Hazard                         | Critical Limit                       | Monitoring                | Corrective Action                          |
|-----|--------------------------------|--------------------------------------|---------------------------|--------------------------------------------|
| 3a  | **Residual ethanol > 50 ppm** → off-flavour, non-compliant | Ethanol ≤ 50 ppm in gum powder       | GC-HS every batch         | Re-dry / re-purge batch; recalibrate dryer |
| 3b  | **Spray dryer outlet too high** → gum degradation / scorch | T-out ≤ 85 °C                         | Continuous RTD            | Reduce inlet temp / feed rate; clean atomiser|
| 3c  | **Allergen cross-contact**     | Dedicated line; CIP between campaigns| Visual CIP check + swab   | Stop line; full CIP repeat                 |
| 3d  | **Ethanol vapour explosion**   | LEL ≤ 25 % in basket centrifuge zone  | Fixed LEL detector        | Emergency vent; stop centrifuge; Evacuate  |

---

## 6. Maintenance Schedule

| Component               | Frequency       | Activity                                                  |
|-------------------------|-----------------|-----------------------------------------------------------|
| Extraction tank agitator| Weekly          | Seal flush; check impeller for wear                       |
| Decanter centrifuge     | 200 hr          | Inspect scroll flights; check bowl hard surfacing         |
| Decanter gearbox        | 1 000 hr        | Change oil (ISO VG 220); inspect ring gear                |
| Vacuum concentrator     | Monthly         | PHE plate cleaning (CIP); check condenser fouling         |
| Basket centrifuge       | 50 cycles       | Replace filter cloth; check brake lining                  |
| Spray dryer atomiser    | 100 hr          | Wheel balance check; bearing temp. logging                |
| Spray dryer bags        | Quarterly       | Replace PTFE bags; check cage integrity                   |
| Ethanol column          | Semi-annual     | Inspect packing for fouling / channelling; ΔP check       |
| LEL sensors             | Quarterly       | Bump-test; calibration                                    |
| CIP circuit             | Monthly         | Verify flow rates, detergent conc., rinse pH              |

---

## 7. Spare Parts Inventory (Minimum Stock)

| Part                          | Qty | Supplier Reference                |
|-------------------------------|-----|-----------------------------------|
| Spray dryer atomiser wheel    | 2   | SD-2000-ATD (OEM)                |
| Spray dryer PTFE filter bags  | 12  | SD-2000-BAG-PTFE                 |
| Decanter scroll tips (tungsten)| 1 set | DC-350-SCR-TIPS             |
| Basket centrifuge cloth (PP)  | 20  | BC-800-CLOTH                     |
| Basket centrifuge brake pads  | 2   | BC-800-BRAKE                     |
| Ethanol column packing (Pall) | 0.5 m³ | PC-300-PALL-SS316            |
| RTD sensors (PT100, 3-wire)   | 5   | RTD-PT100-316                    |
| Concentrator PHE gaskets      | 2 sets | PHE-15-GSK-SS316                 |

---

## 8. Utility Requirements

| Utility          | Connection              | Peak Demand           |
|------------------|-------------------------|-----------------------|
| Electrical       | 400 V, 3-phase, 50 Hz   | 85 kVA                |
| Steam            | 4 bar(g) saturated      | 400 kg/hr             |
| Cooling water    | 25 °C supply, ΔT 10 °C  | 25 m³/hr              |
| Chilled water    | 7 °C supply             | 5 m³/hr (column condenser)|
| Compressed air   | 6 bar(g), oil-free      | 10 Nm³/hr             |
| Water (process)  | Potable, ≤ 5 µS/cm      | 4 m³/hr               |
| Drainage         | Chemical-resistant      | 3 m³/hr               |

---

## 9. Safety & Compliance

- **ATEX Zone 1** (basket centrifuge, ethanol column area, precipitation tank): Ex d IIB T4.
- **ATEX Zone 22** (spray dryer outlet, powder collection): combustible dust rated.
- **Ethanol storage**: Bunded tank farm with fire-water deluge; bonded/grounded.
- **Combustible dust**: Explosion vent panels on spray dryer; bonded bag filter.
- **PPE**: Chemical-resistant gloves + apron for ethanol handling; hearing protection in centrifuge area.
- **LOTO**: Lockout on basket centrifuge door interlock; spray dryer atomiser drive.

---

**Document Owner**: Process Engineering Manager  
**Revision**: 1.0  
**Date**: 2026-07-20  
**CCP-3 Validated**: Production Manager / HACCP Team
