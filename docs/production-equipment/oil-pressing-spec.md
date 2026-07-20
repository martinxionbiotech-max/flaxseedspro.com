# Oil Pressing & Extraction Line — Equipment Specification

## 1. Process Objective

Extract crude flaxseed oil from cleaned, conditioned flaxseed at a sustained throughput of **500 kg/hr** (seed-in) while maintaining oil temperature **≤ 40 °C** to preserve omega-3 (ALA) integrity and prevent oxidative degradation. The line combines **mechanical cold pressing** with **solvent extraction** of the press cake to maximise total oil yield (≥ 98 % recovery). This station is designated **CCP-2** (Critical Control Point — Oil Quality & Solvent Safety).

---

## 2. Equipment Configuration & Flow Diagram

```
Flaxseed (cleaned)
    │
    ▼
[ Pre-heat Conditioner ] ────→ [ SP-300 Screw Press ] ────→ Crude Oil (cold pressed)
    │                                                              │
    ▼                                                              ▼
Press Cake ──────────────→ [ Flaker / Cake Breaker ]      [ Plate Filter (30 µm) ]
    │                                                              │
    ▼                                                              ▼
[ Hexane Extraction Vessel ]                                [ Polish Filter (5 µm) ]
    │                                                              │
    ▼                                                              ▼
[ Miscella (oil+hexane) ] ──→ [ Evaporator ] ──→ [ Stripper ] ──→ Crude Oil to Holding
    │                                                              │
    ▼                                                              ▼
[ Desolventiser / Toaster ] ──→ Meal (≤ 500 ppm hexane)     [ N₂ Blanket Storage ]
```

---

## 3. Equipment Specifications

### 3.1 Pre-Heat Conditioner
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Type                  | Steam-jacketed screw, gentle |
| Throughput            | 600 kg/hr (peak)             |
| Temp. range           | 35 – 55 °C (target 45 °C)   |
| Residence time        | 8 – 12 min                   |
| Heating medium        | Saturated steam @ 2 bar(g)   |
| Material              | SS304 contact surfaces       |

### 3.2 Screw Press — SP-300 (Cold Press)
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Model                 | SP-300 (or equivalent)       |
| Rated capacity        | 500 kg/hr (seed)             |
| Motor power           | 15 kW (TEFC, IE3)            |
| Screw speed           | 20 – 40 rpm (VFD controlled) |
| Oil temperature       | **< 40 °C** (CCP-2 limit)    |
| Cake residual oil     | ≤ 18 % (w/w)                 |
| Pressure at choke     | 50 – 80 MPa                  |
| Cage bars             | Hardened alloy steel (52 HRC)|
| Gearbox               | Helical, oil-flooded         |
| Nozzle / choke        | Hydraulic adjustable         |

### 3.3 Flaker / Cake Breaker
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Roll diameter         | 300 mm                       |
| Roll length           | 600 mm                       |
| Gap setting           | 0.3 – 0.8 mm                 |
| Capacity              | 350 kg/hr (cake in)          |
| Motor                 | 5.5 kW                       |

### 3.4 Solvent Extraction System
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Extractor type        | Perforated-belt / shallow-bed|
| Capacity              | 350 kg/hr (cake/flake)       |
| Solvent               | Commercial hexane (BP 65–70 °C)|
| Solvent-to-solid ratio| 1.0 – 1.2 : 1 (w/w)         |
| Extraction temp.      | 50 – 60 °C                   |
| Miscella conc.        | 20 – 25 % oil                |
| Residual oil in meal  | ≤ 1.0 % (w/w)                |
| Material              | SS304 (all wetted parts)     |

### 3.5 Evaporator (Oil Recovery)
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Type                  | Falling-film evaporator      |
| Heating surface       | 12 m²                        |
| Steam consumption     | 180 kg/hr @ 3 bar(g)         |
| Vacuum level          | −0.85 bar(g)                 |
| Hexane in oil out     | ≤ 1 000 ppm (to stripper)    |

### 3.6 Stripper (Final Desolventising)
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Type                  | Packed column + reboiler     |
| Vacuum level          | −0.92 bar(g)                 |
| Steam sparge          | Live steam, 15 kg/hr         |
| Hexane in crude oil   | **≤ 50 ppm** (food grade)    |
| Oil temp. out         | 60 – 70 °C → cooled to 35 °C |

### 3.7 Desolventiser / Toaster (Meal)
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Type                  | DTDC (Desolventiser-Toaster-Dryer-Cooler)|
| Capacity              | 250 kg/hr meal               |
| Residual hexane       | **≤ 500 ppm**                |
| Steam injection       | 100 kg/hr @ 3 bar(g)         |
| Meal temp. out        | ≤ 50 °C (after cooling)      |

### 3.8 Plate Filter (Cold Press Oil)
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Type                  | Horizontal plate & frame     |
| Filtration area       | 8 m²                         |
| Mesh size             | 30 µm (primary)              |
| Max pressure          | 6 bar                        |
| Material              | SS304 plates, food-gaskets   |
| Capacity              | 250 L/hr (oil)               |

### 3.9 Polish Filter
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Type                  | Bag / cartridge (5 µm)       |
| Housing               | SS304, 2 × 7-element         |
| Capacity              | 250 L/hr                     |
| Design pressure       | 10 bar                       |

### 3.10 Nitrogen Generator (Blanket & Purging)
| Parameter             | Value                        |
|-----------------------|------------------------------|
| Technology            | PSA (Pressure Swing Adsorption)|
| Purity                | 99.9 % N₂                    |
| Capacity              | 20 Nm³/hr                    |
| Dew point             | −40 °C                       |
| Air connection        | 6 bar(g) instrument air      |
| Usage                 | Headspace blanket on oil tanks + hexane system inerting|

---

## 4. Process & Performance Targets

| Metric                          | Target             | Monitoring Method              |
|---------------------------------|--------------------|--------------------------------|
| Cold press throughput           | 500 ± 25 kg/hr     | Load cell (in-feed)            |
| Oil temperature (CCP-2 limit)   | **≤ 40 °C**        | In-line RTD (PID to VFD)       |
| Cold press oil yield            | ≥ 72 %             | Mass balance (seed vs oil)     |
| Total oil recovery (press+extr.)| ≥ 98 %             | Mass balance                   |
| Residual oil in meal            | ≤ 1.0 % (w/w)      | Soxhlet extraction (daily)     |
| Hexane in crude oil             | ≤ 50 ppm           | GC-FID (per batch)             |
| Hexane in meal                  | ≤ 500 ppm          | GC-FID (per shift)             |
| Oil clarity (cold press)        | NTU < 10           | Turbidimeter (after polish)    |

---

## 5. HACCP — CCP-2 Integration

| CCP | Hazard                     | Critical Limit                       | Monitoring                | Corrective Action                          |
|-----|----------------------------|--------------------------------------|---------------------------|--------------------------------------------|
| 2a  | **Oil temp. exceeds 40 °C**→ ALA degradation, PV rise | Oil outlet temp < 40 °C             | Continuous RTD, logged    | Reduce screw speed / feed rate; inspect cooling jacket |
| 2b  | **Hexane leakage** → fire / explosion | LEL < 25 % in atmosphere; hexane in oil ≤ 50 ppm | Fixed LEL gas detector (4 pts) | Emergency vent / deluge; stop feed; evacuate |
| 2c  | **Oxidation during storage**| Headspace O₂ ≤ 2 %                   | O₂ analyser on tank       | Purge with N₂; inspect seal                |

- **Solvent safety**: All electrical equipment in hexane zone rated **Ex d IIB T4** (ATEX / IECEx). Bonding / grounding checked daily. Fixed LEL monitors at extractor, evaporator, and DTDC. Emergency shut-off valves (ESD) at hexane tank farm. Fire deluge system auto-activates at 20 % LEL.

---

## 6. Maintenance Schedule

| Component               | Frequency       | Activity                                                  |
|-------------------------|-----------------|-----------------------------------------------------------|
| Screw press worm & cage | Weekly          | Visual wear check; measure bar gap                        |
| Screw press gearbox     | 2 000 hr        | Replace oil (ISO VG 460); inspect bearings                |
| Plate filter            | Per cycle       | Change plates / gaskets when ΔP > 3 bar                   |
| Polish filter bags      | Per batch / 40 hr | Replace 5 µm bags                                       |
| Evaporator / Stripper   | Monthly         | Inspect tubes for fouling; clean with hot hexane          |
| LEL / gas detectors     | Quarterly       | Bump-test with calibration gas                            |
| N₂ generator            | Semi-annual     | Replace carbon bed filters; check O₂ analyser             |
| All motors              | 6 months        | Grease bearings (NLGI 2), check alignment                 |

---

## 7. Spare Parts Inventory (Minimum Stock)

| Part                          | Qty | Supplier Reference                |
|-------------------------------|-----|-----------------------------------|
| Screw press worm assembly     | 1   | SP-300-WORM (OEM)                |
| Cage bars (set of 12)         | 1   | SP-300-BAR-SET                   |
| Plate filter gaskets (set)    | 2   | PF-8-GSK                         |
| Polish filter bags (5 µm, 7") | 50  | FB-5-70                          |
| Hexane pump mechanical seal   | 2   | MP-25-SEAL                       |
| RTD sensor (PT100, 3-wire)    | 3   | RTD-PT100-316                    |
| LEL sensor head               | 1   | GD-LEL-MK4                       |
| N₂ generator O₂ analyser cell | 1   | PSA-O2-CELL                      |

---

## 8. Utility Requirements

| Utility          | Connection              | Peak Demand           |
|------------------|-------------------------|-----------------------|
| Electrical       | 400 V, 3-phase, 50 Hz   | 55 kVA                |
| Steam            | 3 bar(g) saturated      | 300 kg/hr             |
| Cooling water    | 30 °C supply, ΔT 10 °C  | 5 m³/hr               |
| Instrument air   | 6 bar(g), oil-free      | 30 Nm³/hr             |
| N₂               | 4 bar(g), 99.9%         | 20 Nm³/hr             |
| Drainage         | Chemical-resistant      | 2 m³/hr (condensate + cooling)|

---

## 9. Safety & Compliance

- **ATEX Zone 1** (extractor room, hexane pump area): all Ex d IIB T4 equipment.
- **Grounding**: Continuous conductive floor; all equipment bonded ≤ 10 Ω earth.
- **Fire**: Fixed foam deluge + dry chemical extinguishers (Class B).
- **Lockout/Tagout**: LOTO procedure on screw press hydraulic choke and hexane pumps.
- **PPE**: Flame-retardant coveralls, safety glasses, hexane-resistant gloves in solvent area.

---

**Document Owner**: Process Engineering Manager  
**Revision**: 1.0  
**Date**: 2026-07-20  
**CCP-2 Validated**: Production Manager / HACCP Team
