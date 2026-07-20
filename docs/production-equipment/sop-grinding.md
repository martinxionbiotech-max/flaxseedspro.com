# SOP: Grinding Equipment (Hammer Mill / Cryogenic Grinding)

## 1. Purpose and Scope

This Standard Operating Procedure covers the operation, cleaning, and maintenance of the hammer mill grinding system, including cryogenic nitrogen (N₂) injection for temperature-controlled grinding. It applies to all production operators and maintenance personnel handling flaxseed grinding operations.

## 2. Safety Precautions

### 2.1 Personal Protective Equipment (PPE)
- **Mandatory:** Ear protection (hearing protectors, double protection recommended) — noise exceeds 95 dB(A)
- **Mandatory:** Safety glasses with side shields (or full-face shield during screen changes)
- **Mandatory:** Steel-toed safety boots
- **Mandatory:** Dust mask (N95 minimum; P100 recommended for fine grinding)
- **Mandatory:** Cryogenic gloves (insulated, below-elbow length) when handling N₂ equipment
- **Mandatory:** Safety goggles (not just glasses) when working near N₂ vents
- **Required (when handling chemicals):** Nitrile gloves, chemical splash goggles

### 2.2 Cryogenic N₂ Safety — OXYGEN DEPLETION HAZARD
- **Nitrogen gas (N₂) is odorless, colorless, and displaces oxygen — can cause asphyxiation without warning**
- An **oxygen depletion monitor** MUST be operational in the grinding area at all times during N₂ operation
- Oxygen alarm setpoints:
  - **First alarm (19.5 % O₂):** Evacuate immediately; ventilation check required
  - **Second alarm (18.0 % O₂):** Emergency evacuation; DO NOT enter without SCBA
- If oxygen monitor alarms: EVACUATE immediately, ventilate the area, do NOT re-enter until O₂ ≥20.9 %
- **Never** enter the grinding enclosure or confined space near N₂ injection points without:
  - Continuous O₂ monitoring (personal monitor)
  - Buddy system (second person outside)
  - SCBA if O₂ <19.5 %
- Liquid N₂ can cause severe frostbite — avoid skin contact; use cryogenic gloves
- N₂ vents must be routed outdoors or to a safe exhaust area

### 2.3 Lockout / Tagout (LOTO)
- **Lockout required before:** Screen changes, hammer/internals inspection, bearing maintenance, motor work, N₂ system maintenance
- Verify zero energy state: lock out main power, close and lock N₂ supply valve, depressurize N₂ lines
- Test restart after lockout — confirm no movement
- Personal lock + tag with name, date, and reason

### 2.4 Hot Surfaces
- Hammer mill body and discharge chute can reach 50 °C+ during normal operation
- Motor surface may exceed 60 °C — allow cool-down before contact
- N₂ piping can be cryogenically cold (−196 °C at liquid stage) — identify with warning labels

### 2.5 Rotating Parts & High Energy
- Hammer mill rotor has very high kinetic energy — coast-down time can exceed 5 minutes
- NEVER open access doors until rotor has come to a complete stop
- NEVER reach into the grinding chamber while rotor can move
- Hammers can eject fragments if fractured — ensure chamber door is fully closed and latched

### 2.6 General
- No loose clothing, jewelry, unrestrained hair near rotating shafts
- All guards and interlock switches must be in place and functional
- Fire extinguisher (Class D for metal dust, Class C for electrical) must be present in the grinding area

## 3. Pre-Start Checks

Before starting the grinding system, complete the following checklist. Each item must be verified and initialed.

- [ ] **PPE**: Ear protection (double), dust mask (P100), safety glasses, steel-toed boots, cryogenic gloves (if N₂ in use)
- [ ] **Oxygen Depletion Monitor**: Operational — reading 20.9 % O₂, no alarms active
- [ ] **Guards & Interlocks**: All safety guards in place; door interlock switches functional
- [ ] **Screen Condition**: Screen installed and undamaged — correct mesh size for target grind
- [ ] **Hammer Condition**: Last hammer wear inspection logged (weekly requirement) — hammers above minimum thickness
- [ ] **Rotor Free Rotation**: With power locked out, manually verify rotor spins freely (no binding)
- [ ] **N₂ System** (if cryogenic mode):
  - N₂ supply pressure 5–8 bar
  - Liquid N₂ level sufficient for run (≥25 % in storage tank)
  - All N₂ lines and fittings leak-free (soap test or electronic leak detector)
  - N₂ injection valve in CLOSED position until startup
- [ ] **Temperature Sensors**: All thermocouples functional — verify reading ambient temperature
- [ ] **Discharge System**: Auger / pneumatic conveyor clear, bagging/drum station ready
- [ ] **Feed System**: Feeder clear, no bridging, feed rate controller at minimum
- [ ] **Emergency Stops**: All E-stops tested and functional
- [ ] **Electrical Panel**: MCC breakers on; VFD parameters confirmed for target product
- [ ] **Ventilation**: Area ventilation fans running; N₂ vent line unobstructed and routed outdoors

## 4. Startup Sequence

| Step | Action |
|------|--------|
| 1 | Confirm all Pre-Start Checks are completed and initialed |
| 2 | Announce over intercom: "Starting grinding line" |
| 3 | Start discharge system (auger / pneumatic conveyor / bagging system) |
| 4 | (If N₂ mode) Open N₂ main supply valve — verify line pressure 5–8 bar at regulator |
| 5 | Start hammer mill — run at no-load for 30 seconds; verify smooth operation and no abnormal vibration |
| 6 | Verify no-load amperage is within spec (typically 30–50 % of full-load amps) |
| 7 | (If N₂ mode) Open N₂ injection valve to minimum flow — verify temp drop begins |
| 8 | Start feed system at minimum rate (5–10 % of max) |
| 9 | Monitor mill discharge temperature — allow to stabilize 60 seconds |
| 10 | (If N₂ mode) Adjust N₂ flow to maintain discharge temp within range (30–40 °C) |
| 11 | Increase feed rate in 25 % increments — stabilize 30 seconds between each step |
| 12 | Verify at each step: mill amperage, discharge temperature, N₂ flow rate (if applicable), grind quality |
| 13 | Log startup in equipment logbook: time, operator name, feed rate, mill RPM, N₂ flow (if used), discharge temp |

## 5. Normal Operation Parameters

| Parameter | Normal Range | Alarm Limit | Shutdown Limit |
|-----------|-------------|-------------|----------------|
| Mill discharge temperature (standard) | 30–40 °C | >45 °C | >50 °C |
| Mill discharge temperature (cryogenic) | 10–25 °C | >30 °C | >35 °C |
| Mill motor amperage | 40–65 A (full load: 100 A) | >80 A | >95 A |
| Mill rotor speed (RPM) | 2800–3200 RPM | <2700 or >3300 | <2600 or >3400 |
| N₂ flow rate (cryogenic mode) | 50–150 L/min | >180 L/min or <30 L/min | >200 L/min or <20 L/min |
| N₂ supply pressure | 5–8 bar | <4.5 bar or >8.5 bar | <4 bar or >9 bar |
| Oxygen level (work area) | 20.9 % | <19.5 % (evacuate) | <18.0 % (emergency) |
| Feed rate (flaxseed) | 400–600 kg/h | >700 kg/h | >800 kg/h |
| Grind particle size (D90) | 150–250 µm | >300 µm or <100 µm | >350 µm or <80 µm |
| Vibration level (mill body) | <3.0 mm/s RMS | >5.0 mm/s RMS | >7.0 mm/s RMS |
| Motor bearing temperature | 40–60 °C | >70 °C | >80 °C |
| Screen differential pressure | <50 Pa | >80 Pa | >100 Pa |

## 6. Shutdown Sequence

| Step | Action |
|------|--------|
| 1 | Reduce feed rate to minimum (5–10 % of max) |
| 2 | (If N₂ mode) Close N₂ injection valve — leave main supply valve OPEN (for next startup) |
| 3 | Continue running mill for 2 minutes to clear remaining product from chamber |
| 4 | Stop feed system |
| 5 | Stop hammer mill — allow rotor to coast down completely (5+ minutes) |
| 6 | Do NOT open mill access doors until rotor has completely stopped |
| 7 | Stop discharge system |
| 8 | (If N₂ mode) Close N₂ main supply valve if system will be idle >4 hours |
| 9 | Check oxygen monitor reading — confirm 20.9 % before leaving area |
| 10 | Perform visual inspection of mill exterior — note any abnormal findings |
| 11 | Log shutdown in equipment logbook: time, operator name, run hours, product, N₂ used (total), any issues |

## 7. Emergency Shutdown Procedure

### Activation
Press any red Emergency Stop (E-Stop) or the main panel E-Stop. All drives are cut immediately. **Note:** N₂ flow continues — see below.

### Upon Emergency Shutdown
1. **Do NOT reset** until cause is identified and corrected
2. Announce over intercom: "Emergency shutdown — grinding line stopped"
3. Close N₂ injection valve immediately (manual valve, independent of electrical E-stop)
4. Identify the cause:
   - Fire or explosion (dust explosion risk)
   - Mechanical jam / hammer failure
   - Motor overload / electrical fault
   - Oxygen alarm (O₂ <19.5 %)
   - Personnel injury
   - Excessive temperature (>50 °C discharge)
   - Excessive vibration
5. Secure area — prevent re-entry
6. For **oxygen alarm**: evacuate immediately; do NOT re-enter without SCBA until O₂ verified ≥20.9 %
7. For **fire**: activate E-stop, close N₂, do NOT open mill (oxygen feeds fire), use Class D or CO₂ extinguisher
8. Correct cause (see Troubleshooting Section 9)
9. Clear all personnel before resetting E-stops
10. Follow full Startup Sequence (Section 4) after ESD

### Fire / Dust Explosion
- E-stop immediately
- Close N₂ supply valve
- Do NOT open mill access doors
- Activate fire suppression system if available
- Evacuate area
- Notify plant emergency coordinator immediately

## 8. Cleaning Procedure

### 8.1 Between Products (Changeover Cleaning)

| Step | Action |
|------|--------|
| 1 | Complete full Shutdown Sequence (Section 6) |
| 2 | LOTO equipment — lock main power AND close/lock N₂ supply valve |
| 3 | Verify rotor has come to a complete stop |
| 4 | Open mill access doors |
| 5 | Remove screen — clean with stiff brush and compressed air; inspect for wear |
| 6 | Vacuum clean grinding chamber interior — remove all residual meal and dust |
| 7 | Inspect hammers and wear plates — measure hammer thickness; record in inspection log |
| 8 | Wipe down mill interior with clean, dry, lint-free cloth |
| 9 | Vacuum discharge chute and auger/conveyor system |
| 10 | Reinstall screen (or install new screen for different grind size) |
| 11 | Verify no tools or rags remain in chamber |
| 12 | Close and latch all access doors |
| 13 | Remove LOTO — restore power and N₂ supply |
| 14 | Proceed to Pre-Start Checks (Section 3) |

### 8.2 Daily Cleaning

- Vacuum floor area around hammer mill and discharge station
- Wipe exterior surfaces of mill, motor, and N₂ control panel
- Empty dust collection bins
- Clean feed hopper screen
- Check and clean oxygen monitor sensor (per manufacturer instructions)

### 8.3 Deep Cleaning (Weekly or after 100 operating hours)

| Component | Method |
|-----------|--------|
| Grinding chamber | Remove all hammers and screens; vacuum and brush clean; wipe with food-grade isopropyl alcohol |
| Hammers | Inspect each hammer for wear, cracking, or deformation; measure thickness at wear face |
| Screen | Wash with warm water (40–50 °C) and mild detergent, rinse, dry completely before reinstall |
| N₂ injection nozzle | Remove and inspect for clogging; clean with isopropyl alcohol and compressed air |
| Discharge auger | Full pull-out; clean auger flights and trough |
| Motor cooling fan | Blow out with compressed air — ensure cooling fins are clear |

### 8.4 Chemical Cleaning (As Needed)

| Chemical | Concentration | Contact Time | Rinse Temp | Notes |
|----------|--------------|-------------|------------|-------|
| Food-grade degreaser | 2–5 % v/v | 10–15 min | 50–60 °C | For oily residues in grinding chamber |
| Isopropyl alcohol (99 %) | Neat | Wipe & dry | N/A | For N₂ nozzle, sensors, interior surfaces |
| Sanitizer (quaternary ammonium) | 0.1–0.2 % v/v | 5 min | Cold rinse | Food-contact surfaces only — rinse thoroughly |

## 9. Troubleshooting

| Symptom | Probable Cause | Remedy | Reference |
|---------|---------------|--------|-----------|
| Discharge temperature >50 °C | Feed rate too high; N₂ flow insufficient; hammers dull | Reduce feed rate; increase N₂ flow; inspect/replace hammers | Section 5, Section 10 |
| Mill amperage >95 A | Feed rate too high; hammers worn; screen blocked | Stop mill; reduce feed rate; inspect hammers and screen | Section 6 / 7 |
| Coarse grind (particle size too large) | Screen hole size too large; screen torn; hammers worn | Replace screen with correct mesh; inspect/replace hammers | Section 8.3, Screen change |
| Fine grind (too much dust) | Screen hole size too small; mill speed too high; feed rate too slow | Check screen mesh; verify RPM; adjust feed rate | Section 5 |
| Excessive vibration >7 mm/s | Hammer imbalance; rotor imbalance; bearing wear | Stop immediately; check for broken/missing hammer; rebalance rotor | Section 7 / 10 |
| N₂ flow rate low | Clogged injection nozzle; N₂ supply low; regulator fault | Clean nozzle; check tank level; service regulator | Section 8.3 |
| Oxygen alarm <19.5 % | N₂ leak; inadequate ventilation; N₂ vent blocked | Evacuate; ventilate; find and seal leak; clear vent line | Section 2.2, 7 |
| Mill won't start | Door interlock open; E-stop engaged; VFD fault | Close/latch all doors; reset E-stops; check VFD display | Section 3 |
| Screen blinding / blockage | Product too moist; feed rate too high; screen mesh too fine | Reduce feed rate; dry product to spec; change screen | Section 5 / 8.3 |
| Abnormal noise from chamber | Hammer hitting screen; loose hammer; foreign object | Stop immediately; LOTO; inspect chamber | Section 7 |
| Motor tripping overload | Excessive load; failing bearings; voltage imbalance | Allow motor to cool; check amps/voltage; megger test | Section 10 PM |

## 10. Preventive Maintenance

| Task | Frequency | Action |
|------|-----------|--------|
| Hammer wear inspection | Weekly | Measure thickness at wear face; replace if <80 % of original |
| Screen condition inspection | Weekly | Check for holes, tears, wear; replace if damaged |
| Hammer rotation / flipping | Every 200 operating hours | Rotate hammers to distribute wear evenly |
| Screen replacement | Every 500 operating hours or when damaged | Replace with correct mesh |
| Bearing greasing (mill) | Every 200 operating hours | NLGI #2, 3 pumps per zerk |
| N₂ nozzle cleaning | Monthly | Remove and clean with isopropyl alcohol + compressed air |
| N₂ system leak check | Monthly | Soap test all fittings; repair any leaks |
| O₂ monitor calibration | Monthly | Zero and span calibration per manufacturer spec |
| Vibration analysis | Monthly | Measure mill body vibration; trend data |
| Belt tension check | Every 300 operating hours | Deflection test per spec |
| Hammer replacement | When thickness <80 % original or cracked | Replace entire set (balanced sets only) |
| Rotor balancing | Annually or after any hammer change | Dynamic balance to <1.0 mm/s RMS |
| Motor bearing replacement | Every 8000 operating hours or when noise/vibration present | Replace with OEM bearings |
| Motor insulation test | Annually | Megger at 500 V; min 1 MΩ |
| Full overhaul | Annually or 4000 operating hours | Bearings, hammers, screens, seals, N₂ system, full calibration |
| N₂ storage tank inspection | Per local regulations (typically annually) | Certified N₂ tank inspection |

---

*Document Owner: Production Manager | Last Updated: July 2026 | Review Cycle: Annually*
