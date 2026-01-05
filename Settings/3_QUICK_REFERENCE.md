# Quick Reference & Z-Offset Fix

## Everything You Need At A Glance

---

# 🔴 FIX YOUR SCRATCHING ISSUE (DO THIS FIRST!)

## Problem

- Nozzle scraping on layers 1-2
- Print being pulled off bed
- Started after nozzle/hotend replacement

## Root Cause

**Z-offset miscalibrated** after hardware change

## Solution (Takes 10 minutes)

### Step 1: Auto Bed Leveling

1. On printer or Bambu Studio
2. Run "Auto Bed Leveling"
3. Let it complete

### Step 2: Z-Offset Paper Test

1. Heat nozzle to 200°C, bed to 60°C
2. Home all axes
3. Place regular printer paper on bed
4. Move nozzle to Z=0
5. Slide paper under nozzle
6. Adjust Z-offset until you feel **slight drag**
   - Too tight (can't move paper) → +0.05mm
   - Too loose (no resistance) → -0.05mm
   - **Perfect = like writing on paper**

### Step 3: Test Print

1. Print first layer square (any 100mm x 100mm, 0.2mm tall)
2. Watch first layer:
   - ✅ Flat lines, slight squish, good adhesion = PERFECT
   - ❌ Translucent/super flat = Too close (+0.05mm)
   - ❌ Round lines, gaps = Too far (-0.05mm)
3. Adjust and repeat until perfect

### Step 4: Record Your Value

**Write it down!** Each nozzle type needs its own Z-offset:

- Standard 0.4mm brass + PLA: **\_\_\_** mm
- Hardened 0.4mm + PLA: **\_\_\_** mm
- Hardened 0.4mm + PA6-CF: **\_\_\_** mm

**CRITICAL:** Recalibrate Z-offset every time you change nozzles!

---

# ⚙️ Settings Quick Reference

## PLA Matte

| Setting | Value                      |
| ------- | -------------------------- |
| Nozzle  | 215°C (220°C first)        |
| Bed     | 60°C (65°C first)          |
| Cooling | 100% after layer 4         |
| Speed   | 60mm/s outer, 30mm/s first |
| Walls   | 3 loops                    |
| Infill  | 15% Grid                   |
| Flow    | 0.98                       |

## PLA+

| Setting | Value                      |
| ------- | -------------------------- |
| Nozzle  | 220°C (225°C first)        |
| Bed     | 60°C (70°C first)          |
| Cooling | 90-100% after layer 4      |
| Speed   | 60mm/s outer, 30mm/s first |
| Walls   | 3 loops                    |
| Infill  | 20% Grid                   |
| Flow    | 0.98                       |

## PA6-CF ⚠️

| Setting | Value                         |
| ------- | ----------------------------- |
| Nozzle  | 280°C (285°C first) ⚠️        |
| Bed     | 90°C (95°C first) ⚠️          |
| Cooling | 0-15% MAX ⚠️                  |
| Speed   | 40mm/s outer, 20mm/s first ⚠️ |
| Walls   | 4 loops ⚠️                    |
| Infill  | 40% Gyroid ⚠️                 |
| Brim    | 8mm ⚠️                        |
| Flow    | 0.98                          |

---

# 🆘 Emergency Troubleshooting

## Issue: Nozzle Scratching

**NOW:** Increase Z-offset +0.05mm (live adjust if possible)
**LATER:** Proper Z-offset calibration

## Issue: Print Not Sticking

**NOW:** Clean bed with IPA, increase bed temp +5°C
**LATER:** Full bed wash, check Z-offset

## Issue: Warping (PA6-CF)

**NOW:** DON'T open enclosure, reduce cooling to 0%
**LATER:** Seal enclosure better, increase brim to 10mm

## Issue: Weak Layers (PA6-CF)

**NOW:** CHECK MOISTURE FIRST!
**FIX:** Dry filament 4+ more hours, reduce cooling

## Issue: Stringing

**NOW:** Reduce temp -5°C for current print
**LATER:** Increase retraction to 0.8mm, check moisture

## Issue: Popping/Hissing Sounds

**NOW:** PAUSE - filament has moisture!
**FIX:** Dry filament again (4+ hours at 70°C)

---

# 📋 Pre-Print Checklists

## PLA Prints

- [ ] Bed cleaned with IPA
- [ ] Auto bed leveling done
- [ ] Z-offset calibrated
- [ ] Correct nozzle installed
- [ ] Profile selected (process + filament)

## PA6-CF Prints ⚠️

- [ ] Hardened nozzle installed
- [ ] Z-offset recalibrated for hardened nozzle
- [ ] Filament dried 6+ hours at 70°C
- [ ] Bed: soap/water + IPA clean
- [ ] Magigoo applied and dried (tacky)
- [ ] Enclosure sealed
- [ ] TEST PRINT done successfully (15-20g)
- [ ] Ready for main 300g print

---

# 🎯 Test Prints from MakerWorld

**Go to:** makerworld.com

## For Z-Offset/PLA Testing

- Search: "first layer test" - Do this FIRST!
- Search: "benchy" - Standard validation
- Search: "calibration cube 20mm" - Quick check

## For PA6-CF Testing (BEFORE 300g print!)

- Search: "tensile test specimen" - Strength validation
- Search: "small bracket" - Functional test
- Must test 15-20g before risking 300g!

---

# 💡 Pro Tips

**For PLA:**

1. Clean bed = 90% of adhesion problems solved
2. Z-offset calibration fixes scratching
3. Slow first layer (30mm/s) = better adhesion
4. More top layers (5) = better finish

**For PA6-CF:**

1. **MOISTURE IS ENEMY #1** - always suspect it first!
2. Minimal cooling (0-15%) = strong layers
3. Slow speeds = quality (don't rush!)
4. Don't remove until <40°C = no warping
5. Test print mandatory = saves 300g

**General:**

- Recalibrate Z-offset after ANY nozzle change
- Watch first 5 layers closely
- One change at a time when troubleshooting
- Document what works for your setup

---

# 📞 Quick Decision Tree

**"My nozzle is scratching!"**
→ Increase Z-offset +0.05mm, test again

**"Print won't stick!"**
→ Clean bed, check Z-offset, increase bed temp

**"Setting up PA6-CF"**
→ See full PA6-CF guide, don't skip steps!

**"Which profile to use?"**
→ PLA Matte for aesthetics, PLA+ for strength, PA6-CF for engineering

**"Can I speed things up?"**
→ PLA: Yes, can increase to 80mm/s outer wall
→ PA6-CF: NO! Slow speeds critical for strength

---

# ✅ Success Indicators

**Perfect First Layer:**

- Lines flat but not translucent
- No gaps between lines
- Good adhesion to bed
- No scraping sounds
- Slight texture visible

**Good Print Quality:**

- Smooth surfaces
- Accurate dimensions
- Strong layer bonding (can't separate)
- Minimal stringing
- Clean overhangs

**PA6-CF Success:**

- Test piece impossible to break
- No warping
- Very strong layer bonds
- Ready for main 300g print!

---

# 🎯 Your Action Plan

**TODAY:**

1. Fix Z-offset (see above) - 10 minutes
2. Test with PLA - validate it works

**THIS WEEK:**

1. Download test print from MakerWorld
2. Test PLA Matte profile
3. Test PLA+ profile
4. Verify quality improvement

**BEFORE PA6-CF:**

1. Install hardened nozzle
2. Recalibrate Z-offset
3. Dry filament thoroughly
4. Set up enclosure
5. **DO TEST PRINT** (15-20g)
6. Then attempt 300g main print

---

**You've got everything you need! Start with Z-offset, test with PLA, then tackle PA6-CF! 🚀**
