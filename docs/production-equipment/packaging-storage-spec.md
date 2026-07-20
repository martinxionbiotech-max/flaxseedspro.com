# Packaging & Storage Line — Equipment Specification

## 1. Process Objective

Package finished flaxseed oil, whole seed, meal, and gum powder into consumer-ready and bulk formats at a sustained line rate of **600 bph** (bags/hr, VFFS) while maintaining product quality through controlled-atmosphere packaging and in-line contaminant detection. All packages achieve **O₂ headspace ≤ 2 %** (N₂ flushed), **weight accuracy ± 2 g** (consumer packs), and are 100 % screened for metal and physical contaminants. This station is designated **CCP-5** (Critical Control Point — Metal Contaminants & Package Integrity).

---

## 2. Equipment Configuration & Flow Diagram

```
Dry Product (seed, meal, gum powder)                       Oil Product
    │                                                            │
    ▼                                                            ▼
[ Bulk Filler ] → (FIBC / 1 MT)                         [ Pump / Holding Tank ]
    │                                                            │
    ▼                                                            ▼
[ Bag Filler ] → (10–25 kg bags)                        [ Drum Filler ] → (20–200 L drums)
    │                                                    (N₂ headspace purge)
    ▼
[ VFFS Machine ] ← (roll-stock film, 600 bph)
    │
    ▼
[ N₂ Flush Tunnel ]  →  Bag sealing (O₂ ≤ 2 %)
    │
    ▼
[ Checkweigher ]  →  Reject (± 2 g tolerance)
    │
    ▼
[ Metal Detector ]  →  Reject (Fe 0.5 / NF 0.7 / SS 1.0 mm)
    │
    ▼
[ X-Ray Inspection ]  →  Reject (glass, stone, dense plastic)
    │
    ▼
[ Date Coding / Labelling ]
    │
    ▼
[ Case Packer / Palletiser ]
    │
    ▼
[ Finished Goods Warehouse (ambient, 15–25 °C, RH ≤ 60 %) ]
```

---

## 3. Equipment Specifications

### 3.1 Vertical Form-Fill-Seal (VFFS) Machine
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Type                  | Intermittent-motion VFFS (bag-in-box / stand-up pouch)|
| Line speed            | **600 bph** (10 bags/min, max 70 bpm)|
| Bag size (L × W)      | 150 – 400 mm × 100 – 300 mm          |
| Film width            | 250 – 650 mm                          |
| Film material         | Laminate (PET/Al/PE, PET/met-PE)      |
| Fill volume           | 100 g – 5 kg                          |
| Fill accuracy         | **± 2 g** (via servo-driven auger / volumetric cup + checkweigh feedback)|
| Sealing               | Dual jaw, serrated + flat, temp. control ± 2 °C|
| Sealing temperature   | 140 – 200 °C (depending on film)     |
| Gas flushing          | Integral N₂ purge lance (post-fill, pre-seal)|
| Control               | 10" HMI + PLC (Ethernet/IP)          |
| Material (contact)    | SS316 (auger, cup, funnel); SS304 (frame)|
| Air consumption       | 200 L/min @ 6 bar(g)                  |
| Ex-proof              | Zone 22 rated for combustible dust (powder filling)|

### 3.2 Bag Filler (10–25 kg)
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Type                  | Open-mouth bag filler, gravity + auger trim|
| Capacity              | 6 – 8 bags/min (25 kg)               |
| Weight range          | 5 – 50 kg                             |
| Accuracy              | ± 50 g (gross weigh)                 |
| Bag type              | Woven PP, paper, or PE liner          |
| Stitching             | Sewn closure with tape (DS-9C head)   |
| Material              | SS304 contact                         |

### 3.3 Bulk Filler (FIBC / Big Bags)
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Type                  | Ganries / weigh-frame, vibratory densification|
| Capacity              | 10 – 15 bags/hr (1 000 kg FIBC)      |
| Weight range          | 500 – 1 500 kg                        |
| Accuracy              | ± 0.5 kg                             |
| Filling spout         | Inflatable seal + dust extraction     |
| Loop handling         | Auto loop hang / release              |
| Pallet base           | Integrated fork-pockets for conveyor  |
| Material              | SS304 (contact), carbon steel (frame) |

### 3.4 Drum Filler (Oil)
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Type                  | Automatic net-weight drum filler      |
| Capacity              | 15 – 20 drums/hr (200 L / 180 kg oil)|
| Drum sizes            | 20 L pail – 200 L drum                |
| Fill accuracy         | ± 0.1 kg                             |
| Fill lance            | Sub-surface, rising level (minimise aeration)|
| N₂ purge              | Headspace purge to O₂ ≤ 2 % pre-seal  |
| Tare/bulk/trim cycles | 3-stage: 95 % bulk → 99 % dribble → 100 % trim|
| Material              | SS316 (all wetted surfaces)           |
| Drum handling         | Conveyorised — auto-index, centring, lid placement|
| Ex-proof              | Zone 1 rated (drum filler area, oil mist)|

### 3.5 N₂ Flush Tunnel
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Type                  | Conveyorised tunnel, pre-heated N₂ (blanket + jet)|
| Conveyor width        | 400 mm                               |
| Tunnel length         | 3 000 mm                              |
| N₂ flow               | 50 – 100 Nm³/hr (VFD controlled)      |
| N₂ purity             | 99.9 % (from PSA generator)           |
| Residual O₂ target    | **≤ 2 %** (CCP-5 limit)              |
| O₂ monitoring         | In-line paramagnetic sensor (1 per zone)|
| Temperature control    | Ambient – 40 °C (optional heated N₂ for oil)|
| Exhaust hood          | Integrated, to atmosphere              |
| Air curtain           | Inlet / outlet air curtain to minimise N₂ loss|
| Material              | SS304 tunnel + PTFE belt              |

### 3.6 Checkweigher
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Type                  | Dynamic in-motion, load cell (EMFR)  |
| Conveyor speed        | Up to 80 m/min                        |
| Weight range          | 50 g – 5 kg (VFFS packs)             |
| Accuracy              | ± 0.5 g (3σ at 600 bph)              |
| Reject                | Pneumatic pusher / air-blast (lateral)|
| Displays              | Running average, trend, histograms    |
| Feedback              | Auto-tare compensation to VFFS filler|
| Washdown              | IP65 (hygienic design)                |

### 3.7 Metal Detector
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Type                  | Balanced-coil, multi-frequency        |
| Aperture size         | 300 mm × 150 mm (W × H)              |
| Detection limits      | **Fe: 0.5 mm / NF: 0.7 mm / SS 316: 1.0 mm**|
| Frequency             | Auto-tune (50 – 800 kHz)              |
| Product effect        | Auto-learn / auto-balance             |
| Reject                | Pneumatic pusher (same as checkweigher reject line)|
| Conveyor speed        | Matched to line (up to 80 m/min)      |
| Data logging          | Event log with product image + time stamp|
| Standards             | HACCP / BRC / IFS compliance ready    |
| Washdown              | IP65 (hygienic)                       |

### 3.8 X-Ray Inspection System
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Type                  | Dual-energy X-ray (DX-ray)           |
| Generator             | 160 kV / 1.5 mA, air-cooled           |
| Detector              | Linear diode array (0.4 mm pitch)     |
| Conveyor width        | 500 mm                               |
| Throughput            | Up to 80 m/min                        |
| Detection capability  | **Metals:** Fe ≥ 0.3 mm, SS ≥ 0.4 mm — **Glass:** ≥ 0.5 mm — **Stone:** ≥ 1.0 mm — **Dense plastic:** ≥ 2.0 mm|
| Reject                | Pneumatic pusher + confirmation sensor|
| Software              | Real-time image processing; zone-based algorithm|
| Safety                | Lead shielding — < 1 µSv/hr at surface|
| Data logging          | Full image archive (30 days)          |
| Standards             | GFSI, BRC, IFS                        |

### 3.9 Date Coder / Labeller
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Date coder type       | Thermal inkjet (TIJ) / laser         |
| Print area            | Up to 50 mm × 25 mm                  |
| Print speed           | Up to 100 m/min                      |
| Labeller type         | Roll-fed wraparound + top label (optional)|
| Labeller speed        | Up to 80 labels/min                  |

### 3.10 Case Packer / Palletiser
| Parameter             | Value                                |
|-----------------------|--------------------------------------|
| Case packer type      | Pick-and-place (3-axis servo)        |
| Cases per min         | 8 – 12                                |
| Palletiser type       | Low-level robotic gantry (4-axis)    |
| Pallet load           | Up to 1 200 kg                        |
| Stretch wrapper       | Rotary arm, pre-stretch 250 %         |

---

## 4. Packaging Formats

| Format        | Unit Size        | Packaging Material        | Throughput         |
|---------------|------------------|---------------------------|--------------------|
| Retail pouch  | 250 g – 1 kg     | PET/Al/PE laminate        | 600 bph (VFFS)    |
| Stand-up pouch| 500 g – 2 kg     | Stand-up gusseted, zipper | 400 bph            |
| Bag-in-box    | 5 – 20 kg        | PE liner + corrugated     | 12 bpm             |
| Consumer drum | 20 L (18 kg oil) | HDPE / steel              | 15 – 20 drums/hr  |
| Industrial drum| 200 L (180 kg)   | Steel (epoxy-lined)       | 15 – 20 drums/hr  |
| Bag (woven)   | 10 – 25 kg       | PP woven + PE liner       | 6 – 8 bags/min    |
| FIBC          | 500 – 1 500 kg   | PP bulk bag               | 10 – 15 bags/hr   |

---

## 5. Process & Performance Targets

| Metric                          | Target                    | Monitoring Method              |
|---------------------------------|---------------------------|--------------------------------|
| Line speed (VFFS)               | 600 ± 20 bph             | PLC cycle counter              |
| Fill weight accuracy (VFFS)     | ± 2 g (≤ 1 kg pack)      | Checkweigher (100 %)           |
| Fill weight accuracy (drum)     | ± 0.1 kg                 | Filler load cell               |
| Headspace O₂ (CCP-5 limit)      | **≤ 2 %**                 | In-line paramagnetic O₂ sensor |
| Metal detector sensitivity (Fe) | **0.5 mm** (CCP-5)        | Daily test with test sticks    |
| X-ray: glass / stone detection  | ≥ 99.9 % rejection at 0.5 mm| Weekly challenge test          |
| Package seal integrity          | ≤ 0.1 % leakers          | Vacuum decay / burst test (hourly)|
| N₂ consumption                 | ≤ 100 Nm³/hr              | Flowmeter                      |
| Overall equipment effectiveness | ≥ 85 %                    | OEE dashboard (downtime + speed + quality)|

---

## 6. HACCP — CCP-5 Integration

| CCP | Hazard                         | Critical Limit                       | Monitoring                | Corrective Action                          |
|-----|--------------------------------|--------------------------------------|---------------------------|--------------------------------------------|
| 5a  | **Metal contamination** → physical hazard | Fe ≥ 0.5 mm, NF ≥ 0.7 mm, SS ≥ 1.0 mm | Continuous MD; test sticks hourly | Isolate and re-inspect rejected product; investigate source; recalibrate MD |
| 5b  | **Headspace O₂ > 2 %** → oxidative rancidity | O₂ ≤ 2 % in finished pack            | In-line O₂ sensor (every pack or every 30 sec) | Reject affected packs; check N₂ supply / tunnel seals; adjust N₂ flow |
| 5c  | **Glass / dense contam. > 0.5 mm** | No detectable glass, stone, or dense plastic ≥ 0.5 mm | X-ray (100 % of packs)     | Reject; quarantine preceding 30 min; root cause investigation |
| 5d  | **Weight underfill**            | Net weight ≥ label declared (T1/T2 per weights & measures) | Checkweigher (100 %)       | Auto-reject underweight; trim feedback to VFFS filler |

---

## 7. Maintenance Schedule

| Component               | Frequency       | Activity                                                  |
|-------------------------|-----------------|-----------------------------------------------------------|
| VFFS sealing jaws       | Daily           | Clean residue; check Temp. accuracy; inspect serration    |
| VFFS film unwind        | Weekly          | Check dancer arm, unwind brake                           |
| VFFS auger / cup        | Per product change | Dismantle and clean; verify fill weight                   |
| N₂ tunnel O₂ sensor     | Daily           | Zero & span calibration                                  |
| Checkweigher load cell  | Weekly          | Calibrate with certified weight set                      |
| Metal detector          | **Every 30 min** | Test with Fe/NF/SS test sticks (per BRC/BRCGS protocol)  |
| X-ray detector          | Weekly          | Clean diode array; run daily self-test + weekly challenge |
| X-ray generator         | Semi-annual     | Replace cooling oil; anode inspection                     |
| Drum filler lance seals | 500 cycles      | Replace PTFE seals                                        |
| Drum filler N₂ valve    | Monthly         | Clean and function test                                   |
| Case packer grippers    | Monthly         | Inspect suction cups / mechanical fingers                 |
| Palletiser             | Quarterly       | Check chain tension; lubricate linear guides              |
| Stretch wrapper         | Semi-annual     | Replace pre-stretch belts; calibrate tension              |

---

## 8. Spare Parts Inventory (Minimum Stock)

| Part                          | Qty | Supplier Reference                |
|-------------------------------|-----|-----------------------------------|
| VFFS sealing jaw (serrated)   | 2   | VFFS-SJ-400 (OEM)                |
| VFFS film cutter blade        | 5   | VFFS-FCB-650                     |
| N₂ O₂ sensor cell (paramagnetic)| 1  | O2-PM-CELL                       |
| Checkweigher load cell        | 1   | CW-LC-30KG                       |
| Metal detector test sticks    | 1 set | MD-TEST-FE/NF/SS              |
| MD reject pusher solenoid     | 2   | MD-SOL-PN                        |
| X-ray diode array segment     | 1   | XR-DIODE-0.4MM                   |
| Drum filler PTFE seal kit     | 2   | DF-SEAL-KIT                      |
| Drum filler fill lance        | 1   | DF-LANCE-316                     |
| Case packer suction cup       | 20  | CP-SCUP-30                       |
| N₂ tunnel air curtain fan     | 1   | NT-FAN-400                       |

---

## 9. Utility Requirements

| Utility          | Connection              | Peak Demand           |
|------------------|-------------------------|-----------------------|
| Electrical       | 400 V, 3-phase, 50 Hz   | 45 kVA                |
| N₂               | 4 bar(g), 99.9 %        | 100 Nm³/hr            |
| Compressed air   | 6 bar(g), oil-free      | 500 L/min (VFFS, rejectors, case packer)|
| Dust extraction  | 2 000 m³/hr @ −1.5 kPa | Bulk fill + bag filler points|

---

## 10. Safety & Compliance

- **ATEX Zone 22**: VFFS area (gum/meal powder); bag filler station; bulk filler dust extraction.
- **ATEX Zone 1**: Drum filler station (oil mist zone).
- **X-ray safety**: Annual survey per UK HSE IRR17 / US FDA 21 CFR 1020.40 — public limit < 1 µSv/hr at 10 cm.
- **Metal detector**: Self-test log maintained for BRC / GFSI audits; MD belt interlocked to reject gate.
- **LOTO**: Checkweigher belt drive, VFFS seal jaw servo, drum filler indexing, X-ray conveyor.
- **PPE**: Cut-resistant gloves for film handling; ear plugs (> 85 dB(A) in case packer area); dosimeter badges for X-ray area.
- **Weights & Measures**: All checkweighers verified to Class X(1) accuracy with traceable standards (monthly).

---

## 11. Warehouse Storage Conditions

| Parameter             | Target                    | Monitoring                |
|-----------------------|---------------------------|---------------------------|
| Ambient temperature   | 15 – 25 °C                | Data-logger (hourly)      |
| Relative humidity     | ≤ 60 %                    | Hygrometer (continuous)   |
| FIFO / FEFO           | By production date        | WMS (barcode scan)        |
| Pest control          | IPM programme (monthly)   | External contractor       |
| Inventory system      | Real-time WMS             | SAP / ERP integration     |

---

**Document Owner**: Process Engineering Manager  
**Revision**: 1.0  
**Date**: 2026-07-20  
**CCP-5 Validated**: Production Manager / HACCP Team
