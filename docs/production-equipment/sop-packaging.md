# SOP-PACKAGING: VFFS Packaging, Checkweighing, Metal Detection & X-Ray Inspection

**Document No:** SOP-PK-001  
**Version:** 1.0  
**Effective Date:** 2026-07-20  
**Department:** Packaging  
**Scope:** This procedure covers vertical form-fill-seal (VFFS) packaging operations, N₂ flush verification, checkweighing, metal detection, X-ray inspection, film splice handling, and associated troubleshooting for flaxseed products.

---

## 1. Safety

### 1.1 Machine Safety
- Only trained and authorised personnel may operate packaging equipment.
- Ensure all guarding, interlocks, and light curtains are functional.
- Lockout/tagout (LOTO) required for any cleaning, maintenance, or jam clearing.
- **Crush hazard:** Keep hands clear of sealing jaws, forming tube, and film carriage.
- **Burn hazard:** Seal jaws operate at 185±5°C. Allow 10 minutes to cool before accessing.

### 1.2 N₂ Safety (Asphyxiation Risk)
- N₂ is an odourless, colourless gas that displaces oxygen.
- Packaging area must have O₂ deficiency monitors (alarm at 19.5% O₂).
- Ensure adequate ventilation. If O₂ alarm sounds: evacuate immediately.
- N₂ supply lines must be labelled and leak-checked quarterly.

### 1.3 Personal Protective Equipment (PPE)
- Safety glasses, cut-resistant gloves (film handling), steel-toed boots.
- Hearing protection if cumulative noise >85 dBA.
- Dust mask (N95) if handling dusty product at infeed.

### 1.4 X-Ray Safety
- **Do not** reach into the X-ray cabinet while the unit is energised.
- Interlock failure: if X-ray stays on when cabinet door is opened, evacuate area and call maintenance.
- Annual radiation survey required. Wear dosimeter badge if applicable.

---

## 2. VFFS (Vertical Form-Fill-Seal) Machine Operation

### 2.1 Film Loading
1. Select correct film roll per product specification (check width, gauge, and print registration).
2. Position roll on unwind shaft; lock into place with cones.
3. Thread film through tension rollers, dancer arm, and forming tube:
   - Follow the path diagram on the machine panel.
   - Ensure film passes straight through all rollers (no twists).
4. Dancer arm should be at approximately 45° angle after threading.
5. Set web tension: 15–25 N (adjust as needed for film type).
6. Verify print registration mark sensor is aligned with registration marks.

### 2.2 Seal Jaw Temperature Setup
1. Turn on main power and heater switches.
2. Set **back seal jaw temperature** to 185°C.
3. Set **front seal jaw temperature** to 185°C.
4. Allow 15 minutes warm-up time.
5. **Acceptable range:** 185 ± 5°C (180–190°C).
6. Verify temperature with external contact pyrometer (not just the display).
7. If temperature is outside range, adjust setpoint and recalibrate sensor.
8. Record jaw temperatures on **PKG-LOG-001** before each production run.

### 2.3 Bag Length Setting
1. Measure required bag length from product specification (e.g., 250 mm for 500 g bags).
2. Set bag length on the HMI (touchscreen or encoder setting).
3. **Film advance test:** Run 5 empty cycles and measure actual bag length.
4. Adjust if measured length deviates >2 mm from target.
5. Verify end seal is centred on bag (equal top and bottom seal margins).

### 2.4 Startup Sequence
1. Verify product hopper has sufficient material.
2. Ensure bag chute and conveyor are clear.
3. Start VFFS in **jog mode** — run 2–3 empty bags.
4. Check seal quality on empty bags:
   - Seal width: ≥3 mm.
   - No pinholes, wrinkles, or burn-through.
5. Start **main run**.
6. Start product feed (auger or volumetric filler).
7. Verify first 10 bags visually — seal quality, fill weight, print registration.
8. If first 10 bags are acceptable, start auto-run.

---

## 3. N₂ Flush Verification

### 3.1 Purpose
N₂ flush removes oxygen from the bag headspace to extend product shelf life and protect oil quality.

### 3.2 O₂ Analyzer Calibration
1. Calibrate O₂ analyser daily before production:
   - **Zero gas:** 99.999% N₂ — reading should show 0.0% O₂.
   - **Span gas:** Ambient air — reading should show 20.9% O₂.
2. Adjust calibration if readings deviate >0.1% from expected.
3. Record calibration on **PKG-LOG-001**.

### 3.3 Headspace O₂ Verification
1. Insert needle probe through seal area of a freshly produced bag.
2. Read O₂ level on analyser when stable (10–15 seconds).
3. **Acceptance criteria:** O₂ ≤2.0% in headspace.
4. Test at start of run, after film splice, after any machine stoppage >5 minutes, and every 30 minutes during production.
5. If O₂ >2.0%:
   - Increase N₂ flow rate.
   - Check N₂ supply pressure (target 2–3 bar at machine).
   - Verify N₂ injection nozzle position (should be inside forming tube).
   - Check for leaks in the forming tube area.

---

## 4. Checkweigher Setup

### 4.1 Configuration Parameters
| Parameter | Setting |
|---|---|
| Tare weight | 0 g (dynamic tare; measure 10 empty bags) |
| Target weight | Per product spec (e.g., 500 g) |
| Upper reject limit | Target + 5 g |
| Lower reject limit | Target - 3 g |
| Tare interval | Every 50 bags (or per manufacturer) |

### 4.2 Calibration Procedure
1. Place certified calibration weight (e.g., 500 g) on the weigh cell.
2. Initiate auto-calibration from HMI.
3. Verify reading is within ±0.5 g of calibration weight.
4. Repeat with a 200 g and 800 g weight to verify linearity.
5. Calibrate at start of each shift and after belt changes.

### 4.3 Rejection System
- **Pneumatic pusher or drop-out reject:** Verify actuation daily.
- Confirm reject bin is empty at start of run.
- Run a test reject (manual trigger) to verify timing and position.
- Check that reject gate opens completely and closes fully.

### 4.4 Weight Drift Monitoring
- Monitor weight trend on HMI display.
- If 3 consecutive bags are trending toward limit, check filler adjustment.
- If 2 consecutive bags are rejected, stop line and investigate.

---

## 5. Metal Detector Operation

### 5.1 Setup Parameters
| Parameter | Setting |
|---|---|
| Ferrous (Fe) threshold | 0.5 mm |
| Non-ferrous (NF) threshold | 0.7 mm |
| Stainless steel (SS) threshold | 1.0 mm |
| Product effect compensation | Auto-learn per product type |

### 5.2 Product Effect Compensation
1. Run a bag of product through the metal detector 10 times.
2. Record the phase and amplitude of the product signal.
3. Set the compensation to auto-phase-shift to cancel the product signal.
4. Verify with a test wand: all test pieces must be detected with product present.
5. Re-run compensation if product formulation changes.

### 5.3 Test Wand Procedure
1. Select test wand with Fe (0.5 mm), NF (0.7 mm), and SS (1.0 mm) test pieces.
2. **Sequence (must pass all):**
   a. Pass Fe wand through centre of aperture — must reject.
   b. Pass NF wand through centre — must reject.
   c. Pass SS wand through centre — must reject.
   d. Pass each wand at left, centre, and right of belt — all must reject.
3. Test at:
   - Start of each production run.
   - Every 1 hour during production.
   - After any metal detector adjustment.
4. If any test fails: stop line, recalibrate, and re-test.
5. Record all test results on **PKG-MET-LOG-002**.

### 5.4 Handling Rejected Bags
1. Stop line when reject occurs.
2. Place the rejected bag in a quarantine container.
3. Run the bag through again in detection mode.
4. If confirmed reject: document and set aside for investigation.
5. If false reject: investigate and recalibrate.

---

## 6. X-Ray Inspection System

### 6.1 Test Piece Verification
1. Use certified test pieces: stainless steel (0.5 mm), glass (1.0 mm), ceramic (1.0 mm), dense plastic (2.0 mm).
2. Place test piece in a bag of product.
3. Run bag through X-ray — must detect and reject.
4. Test at each shift start and every 2 hours.
5. Record results on **PKG-XRY-LOG-003**.

### 6.2 X-Ray Image Review
- Operator must visually review the X-ray image of each rejected bag on the display.
- Confirm contaminant visibility or mark as false reject.
- Log false reject rate — if >0.5%, recalibrate sensitivity.

---

## 7. Film Splice Procedure

### 7.1 When to Splice
- Film roll end is approaching (last ~10 m).
- Film defect detected (wrinkle, tear, print error).

### 7.2 Splice Procedure
1. Stop VFFS machine at a convenient point (between cycles).
2. Bring new film roll to the unwind station.
3. Overlap the end of the old film and the start of the new film by 30 mm.
4. Use **splice tape** (approved type only) across the full film width.
5. Apply tape on both sides of the film (front and back).
6. Check that the registration marks on the new film are correctly aligned.
7. Re-thread through dancer arm and forming tube if needed.
8. Restart in **jog mode** — verify new film feeds correctly.
9. Run 2 bags and visually inspect: seal quality, registration, print.
10. Inspect splice area — make sure it passes through without jamming.

### 7.3 Post-Splice Checks
- Verify N₂ headspace O₂ (re-test per Section 3.3).
- Check seal temperature (re-verify with pyrometer).
- Metal detector test wand check.
- Checkweigher — verify first 5 bags are within tolerance.

---

## 8. Cleaning Procedures

### 8.1 Between Product Changeovers
1. LOTO the packaging line.
2. Remove all product from hopper, auger, and forming tube.
3. Wipe down forming tube, seal jaws, and bag chute with clean damp cloth.
4. Vacuum product dust from all surfaces.
5. Clean checkweigher belt with approved cleaner (isopropyl alcohol wipes).
6. Clean metal detector aperture — no metal debris, dust, or product buildup.
7. Clean X-ray conveyor belt with damp cloth.

### 8.2 Deep Cleaning (Weekly)
1. Remove film roll, unwind shaft, and tension rollers.
2. Clean seal jaws with a brass brush (do not use abrasives).
3. Lubricate seal jaw bushings with food-grade grease.
4. Clean and inspect film dancer arm bearings.
5. Blow out control panel with compressed air (low pressure, 2 bar max).
6. Clean checkweigher weigh cell area — gentle vacuum only, no compressed air.
7. X-ray: wipe down cabinet interior, check seals/gaskets.

---

## 9. Troubleshooting

| Problem | Possible Cause | Corrective Action |
|---|---|---|
| **Weak seals (leakers)** | Jaw temperature too low | Increase to 185°C; verify with pyrometer |
|  | Jaw temperature too high (burning) | Decrease to 180°C; check seal dwell time |
|  | Jaw pressure insufficient | Adjust pneumatic pressure regulator to 4–5 bar |
|  | Film contamination (oil/dust) | Clean jaws with brass brush |
|  | Worn or damaged seal jaws | Inspect for nicks; replace if damaged |
| **Bag misfeed / jamming** | Film tension too high/low | Adjust dancer arm tension to 15–25 N |
|  | Incorrect bag length setting | Remeasure and adjust |
|  | Registration mark misaligned | Reposition sensor; clean sensor lens |
|  | Forming tube worn / rough | Polish or replace forming tube |
|  | Splice tape caught on roller | Check splice quality; re-tape if needed |
| **Weight drift** | Product density change | Check incoming product; adjust auger fill parameters |
|  | Auger wear | Inspect auger flights; replace if worn >10% |
|  | Filler timing drift | Re-sync auger motor |
|  | Checkweigher calibration drift | Re-calibrate with certified weight |
|  | Belt speed variation | Check drive belt tension; clean pulleys |
| **False metal detector rejects** | Product effect compensation incorrect | Re-run product effect compensation (Section 5.2) |
|  | Vibration from nearby equipment | Isolate metal detector from vibration; check mounting |
|  | Belt noise (metal particles on belt) | Clean belt; replace if worn |
|  | Environmental electrical noise | Check cable shielding; relocate nearby motors |
|  | Sensitivity set too high | Increase threshold by 10% and re-test |
| **Metal detector fails test wand** | Sensitivity drift | Recalibrate per manufacturer |
|  | Aperture blockage | Remove all product from aperture; clean |
|  | Board fault | Call maintenance for diagnostics |
| **X-ray image quality poor** | Belt misalignment | Centre belt on rollers |
|  | Detector drift | Run auto-calibration |
|  | Product too dense | Increase X-ray power (if allowed by spec) |
|  | Contaminant at edge of belt | Check product spread — centre on belt |
| **N₂ headspace O₂ >2%** | N₂ supply pressure low | Verify 2–3 bar at machine |
|  | N₂ injector nozzle displaced | Reposition inside forming tube |
|  | Flow rate insufficient | Increase N₂ flow rate |
|  | Bag seal leaking | Check seal quality per "Weak seals" above |
|  | O₂ analyser calibration drift | Recalibrate per Section 3.2 |
| **Film wrinkle in seal** | Film width mismatch | Verify film matches forming tube |
|  | Forming tube size incorrect | Change to correct diameter |
|  | Uneven jaw pressure | Adjust pneumatic balance |
|  | Dancer arm flutter | Check air damping on dancer |

---

## 10. Documentation

- **PKG-LOG-001:** Production log (jaw temps, N₂ O₂ readings, checkweigher setup, film roll ID).
- **PKG-MET-LOG-002:** Metal detector test results (hourly or per event).
- **PKG-XRY-LOG-003:** X-ray test piece verification (shift start and 2-hourly).
- **PKG-REJ-LOG-004:** Rejected bag log (weight rejects, metal rejects, X-ray rejects).
- **CLEAN-LOG-005:** Cleaning records (per changeover and weekly deep clean).

---

## 11. Appendix: Acceptable Quality Criteria (Product Release)

| Parameter | Specification |
|---|---|
| Fill weight | Target ± 3 g (e.g., 500 ± 3 g) |
| Bag appearance | No wrinkles, clean seals, correct print |
| Seal width | ≥3 mm, continuous, no pinholes |
| Headspace O₂ | ≤2.0% |
| Metal contamination | None detectable (Fe 0.5, NF 0.7, SS 1.0 mm) |
| X-ray detectable contaminants | None detectable (SS 0.5, glass 1.0, ceramic 1.0 mm) |
| Bag length | Target ± 2 mm |

---

*End of Document*
