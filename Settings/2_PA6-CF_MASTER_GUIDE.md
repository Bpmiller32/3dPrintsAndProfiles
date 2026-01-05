# PA6-CF Complete Print Guide + Test Files

## Everything for Your Critical 300g G69+Frame Print

---

# ⚠️ PA6-CF Critical Requirements

**NON-NEGOTIABLE:**

- 0.4mm hardened steel nozzle (carbon fiber destroys brass)
- Filament dried 6+ hours at 70°C (PA6 absorbs moisture instantly)
- Fully enclosed printer (tent, target 40-50°C chamber)
- Magigoo or equivalent adhesive
- DO NOT REMOVE until cooled to <40°C
- **TEST PRINT FIRST** (only 200g margin on 500g spool!)

---

# Pre-Print Checklist (Day Before)

## T-24 Hours

- [ ] Start drying PA6-CF in filament dryer (70°C, 6+ hours minimum)
- [ ] Test enclosure seals with PLA print
- [ ] Install hardened 0.4mm nozzle
- [ ] Clean bed: soap/water, rinse, dry, then IPA

## T-1 Hour

- [ ] Recalibrate Z-offset for hardened nozzle (CRITICAL!)
- [ ] Apply Magigoo, let dry until tacky (5-10 min)
- [ ] Seal enclosure completely
- [ ] Load dried filament directly from dryer to printer
- [ ] Verify settings: 280/285°C nozzle, 90/95°C bed

## T-0 (Start Print)

- [ ] Purge 50mm, check for moisture (popping/hissing)
- [ ] If moisture detected: STOP, dry more
- [ ] Start print
- [ ] **WATCH FIRST 10 LAYERS LIKE A HAWK**

---

# During Print Monitoring

**Minutes 0-5:** DON'T LEAVE

- First layer MUST stick perfectly
- No lifting, no warping
- If problems: STOP immediately

**Minutes 5-30:** Check every 5 minutes

- Monitor adhesion
- Listen for moisture (popping)
- Check corners for lifting

**Hour 1-2:** Check every 30 minutes

- Verify no warping
- Temperature stable
- Enclosure staying warm

**Remaining print:** Check hourly

- General monitoring
- Don't open enclosure!

---

# Emergency Stop Criteria

**STOP PRINT if you see:**

- ❌ First layer not sticking
- ❌ Corners lifting
- ❌ Popping/hissing sounds (moisture!)
- ❌ Major warping starting
- ❌ Nozzle hitting/catching on print

**Better to waste 5-10g than 300g!**

---

# Post-Print Protocol

## Cooling (CRITICAL!)

1. **Leave in enclosure with door CLOSED**
2. Let cool naturally to <40°C (takes 1-2 hours)
3. PA6 is soft when hot - will warp if removed early
4. Be patient!

## Removal

1. Once fully cool, remove carefully with scraper
2. Clean Magigoo with warm water
3. Inspect part for warping/defects

## Storage

- PA6-CF absorbs moisture from air
- If not using immediately, store with desiccant
- Dry again before next print

---

# Common PA6-CF Issues & Fixes

## Poor Bed Adhesion

- **Fix:** More Magigoo, increase bed to 100°C, increase brim to 10mm

## Warping

- **Fix:** Check enclosure seals, reduce cooling to 0%, larger brim

## Weak Layers (Can pull apart)

- **Fix:** CHECK MOISTURE (95% cause!), reduce cooling, increase nozzle 5°C

## Stringing

- **Fix:** Filament wet (dry more), increase retraction to 1.0mm

## Popping/Hissing During Print

- **Fix:** MOISTURE! Stop, dry filament 4+ more hours

---

# Test Prints from MakerWorld

## Before Your 300g Print - DO THIS!

### Test Print 1: PA6-CF Strength Bar ⭐

**MakerWorld Link:** Search "tensile test specimen" or "strength bar"

- **Purpose:** Validate layer adhesion and settings
- **Size:** 60mm bar, 15-20g
- **Test:** Try to break it - should be VERY strong
- **If passes:** Settings are good, proceed to main print

### Test Print 2: Small Bracket

**MakerWorld Link:** Search "small bracket test" or "corner bracket"

- **Purpose:** Real-world functionality test
- **Size:** 30-40mm, 15-20g
- **Test:** Check for warping, strength, accuracy

---

# PLA Test Prints from MakerWorld

## For Validating PLA Profiles

### 3DBenchy ⭐ (The Standard)

**MakerWorld Link:** Search "benchy" or "3D benchy"

- **Purpose:** Tests everything - overhangs, bridges, details
- **Size:** ~13g, ~2 hours
- **What to look for:** Smooth surfaces, good overhangs, no stringing

### Calibration Cube

**MakerWorld Link:** Search "calibration cube 20mm" or "xyz cube"

- **Purpose:** Dimensional accuracy, flow calibration
- **Size:** 20mm cube, ~8g, 30 minutes
- **Test:** Measure with calipers - should be exactly 20mm

### First Layer Test

**MakerWorld Link:** Search "first layer test" or "bed level test"

- **Purpose:** Z-offset and adhesion validation
- **Size:** 100mm square, one layer, 5 minutes
- **Critical:** Do this FIRST to fix scratching!

### Overhang Test

**MakerWorld Link:** Search "overhang test" or "overhang challenge"

- **Purpose:** Verify cooling settings
- **Features:** Progressive overhangs 15° to 70°

---

# How to Download from MakerWorld

1. Go to **makerworld.com**
2. Search for model name (use quotes above)
3. Download STL
4. Import to Bambu Studio
5. Select your custom profile
6. Slice and print!

---

# Your Specific G69+Frame Print

## Critical Info

- **File:** G69+Frame+V2.3mf (Plate 3)
- **Material needed:** 300g PA6-CF
- **Spool size:** 500g total
- **Margin for error:** Only 200g!
- **Stakes:** HIGH - can't afford to fail

## Before Main Print

1. **DO TEST PRINT** (15-20g) - validates everything
2. If test succeeds: Proceed with confidence
3. If test fails: Troubleshoot before wasting material

## Print Strategy

- Use PA6-CF profile exactly as specified
- Don't deviate from settings
- Monitor closely
- Trust the process (slow speeds are intentional!)

---

# Troubleshooting Decision Tree

**Issue:** First layer not sticking
→ More Magigoo + increase bed to 100°C + larger brim

**Issue:** Warping/corners lifting
→ Seal enclosure gaps + reduce cooling to 0% + increase brim

**Issue:** Layers weak/separating
→ **CHECK MOISTURE FIRST!** + reduce cooling + increase temp 5°C

**Issue:** Popping sounds
→ FILAMENT WET - stop and dry more

**Issue:** Stringing
→ Filament likely wet - dry again + increase retraction

**Issue:** Poor surface finish
→ Reduce outer wall speed to 35mm/s + check moisture

---

# Quick Reference

## PA6-CF Settings Summary

| Setting | Value        |
| ------- | ------------ |
| Nozzle  | 280/285°C    |
| Bed     | 90/95°C      |
| Cooling | 0-15% MAX    |
| Speed   | 40mm/s outer |
| Walls   | 4 loops      |
| Infill  | 40% Gyroid   |
| Brim    | 8mm          |

## Critical Success Factors

1. **Moisture control** - #1 cause of failure
2. **Minimal cooling** - critical for layer bonding
3. **Slow speeds** - quality over time
4. **Enclosure** - prevents warping
5. **Patience** - don't rush any step

---

# Success Checklist

**Pre-Print:**

- [ ] Hardened nozzle installed
- [ ] Z-offset recalibrated
- [ ] Filament dried 6+ hours
- [ ] Bed cleaned and Magigoo applied
- [ ] Enclosure sealed
- [ ] Test print completed successfully

**During Print:**

- [ ] First layer perfect
- [ ] No warping observed
- [ ] No moisture sounds
- [ ] Temperature stable
- [ ] Monitoring schedule followed

**Post-Print:**

- [ ] Cooled to <40°C before removal
- [ ] Part dimensionally accurate
- [ ] No warping
- [ ] Layers very strong
- [ ] Ready to use!

---

**You've got this! Follow the steps, don't skip the test print, and you'll get a perfect part! 🎯**
