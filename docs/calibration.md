# Calibration Procedures

## Calibration Overview

Calibration ensures accurate color, white balance, and depth measurements. Regular calibration is recommended for consistent results.

**Calibration Frequency:**
- After first setup: 2-3 times
- Weekly for daily use: Once per week
- Monthly for occasional use: Once per month
- After temperature change: After 30+ minutes
- After moving camera: Before critical work

## Pre-Calibration Checklist

- [ ] Camera powered on and warmed up (5 minutes)
- [ ] USB connection stable
- [ ] Lighting conditions stable
- [ ] Calibration plate clean and undamaged
- [ ] No shadows on calibration surface
- [ ] Room temperature stable
- [ ] Sufficient disk space available

## White Balance Calibration

### Method 1: Using White Reference Card

**Required Materials:**
- White balance reference card (included)
- 18% gray card (optional, for advanced calibration)

**Procedure:**

1. **Position Reference Card**
   - Place white card in front of camera
   - Ensure full coverage of frame
   - Position at normal working distance
   - Avoid shadows on card
   - Ensure even lighting

2. **Capture Reference Image**
   - Open RobotAI Camera software
   - Navigate to **Calibration > White Balance**
   - Click **Capture White Reference**
   - Camera captures image of white card
   - Do not move card during capture

3. **Apply Calibration**
   - Software analyzes white reference
   - Click **Apply Calibration**
   - "Success" message confirms
   - New white balance saved

4. **Verify Results**
   - Remove white card
   - Check live view colors
   - Colors should appear neutral
   - Test on neutral gray object

### Method 2: Manual Color Temperature

**For Known Lighting Conditions:**

1. Determine color temperature of lighting
2. Open **Settings > White Balance > Manual**
3. Enter color temperature in Kelvin
4. Apply to current settings

**Common Color Temperatures:**
- Daylight: 5500K
- Cloudy: 6500K
- Tungsten bulb: 3200K
- Fluorescent: 4500K
- LED: 3000-5600K (varies)

## Color Accuracy Calibration

### Using ColorChecker Passport

**Required Materials:**
- X-Rite ColorChecker Passport or similar
- Neutral lighting
- Calibration software (included)

**Procedure:**

1. **Capture ColorChecker Image**
   - Position ColorChecker in scene
   - Ensure even lighting
   - No shadows on card
   - Fill ~50% of frame
   - Capture image

2. **Analyze Color Data**
   - Open **Calibration > Color Accuracy**
   - Load ColorChecker image
   - Software identifies color patches
   - Calculates color accuracy
   - Generates correction profile

3. **Apply Color Profile**
   - Review color analysis results
   - Delta E values < 2 are excellent
   - Click **Generate Profile**
   - Profile applied to camera
   - Save profile with date

### Verification

1. Capture new ColorChecker image
2. Compare with calibration target
3. Colors should match within Delta E < 1

## Depth Calibration

### Depth Accuracy Calibration

**Required Materials:**
- Calibration plate (included)
- Flat, rigid surface
- Level surface
- Ruler or measuring tape

**Procedure:**

1. **Prepare Calibration Setup**
   - Place calibration plate on flat surface
   - Ensure plate is level
   - Position camera perpendicular to plate
   - Measure distance: 300mm to 1500mm
   - Mark measurement distance

2. **Capture Calibration Data**
   - Open **Calibration > Depth**
   - Enter actual distance to plate
   - Click **Capture Calibration**
   - Camera captures depth map
   - Process multiple distances

3. **Multi-Point Calibration**
   - Capture at 5-7 different distances
   - Recommended: 300mm, 500mm, 700mm, 900mm, 1100mm, 1300mm, 1500mm
   - Each point improves accuracy
   - Allow 10 seconds between captures

4. **Analyze Results**
   - Software calculates calibration curve
   - Displays accuracy at each distance
   - Average accuracy should be < ±1mm
   - Graphs show any systematic errors

5. **Apply Calibration**
   - Click **Apply Depth Calibration**
   - New calibration saved
   - Restart software to apply fully

### Depth Quality Verification

**After Calibration:**

1. Capture test objects at various distances
2. Compare camera measurements to actual
3. Accuracy should meet specifications
4. Document results for reference

## Geometric Calibration

### Lens Distortion Calibration

**Required Materials:**
- Flat checkerboard pattern
- Printed or displayed pattern
- Flat surface for mounting

**Procedure:**

1. **Capture Distortion Reference**
   - Display checkerboard pattern
   - Fill entire camera frame
   - Capture multiple angles
   - Tilt pattern ±30 degrees
   - Capture 5-10 images

2. **Analyze Distortion**
   - Open **Calibration > Geometric**
   - Load checkerboard images
   - Software detects grid points
   - Calculates distortion coefficients
   - Identifies barrel or pincushion distortion

3. **Apply Correction**
   - Review distortion analysis
   - Click **Calculate Distortion Map**
   - Apply correction to all captures
   - Save calibration data

## Thermal Calibration

### Temperature Compensation

Camera automatically compensates for temperature changes, but manual calibration improves accuracy.

**Procedure:**

1. **Cold Calibration (below 10°C)**
   - Allow camera to stabilize at cold temperature
   - Open **Calibration > Thermal**
   - Click **Capture Cold Reference**
   - Camera records baseline

2. **Warm Calibration (above 35°C)**
   - Allow camera to warm up
   - Click **Capture Warm Reference**
   - Records warm baseline

3. **Apply Thermal Compensation**
   - Software creates compensation curve
   - Automatically adjusts for temperature
   - Improves accuracy across temperature range

## Periodic Calibration Validation

### Weekly Validation

1. Capture white balance reference
2. Compare to stored profile
3. If Delta E > 2, perform full white balance calibration
4. Document results

### Monthly Comprehensive Check

1. Perform white balance calibration
2. Perform color accuracy calibration
3. Verify depth accuracy at 3 distances
4. Check geometric distortion
5. Document all results
6. Generate calibration report

## Calibration Management

### Save Calibration Profile

1. After successful calibration
2. Click **Save Calibration As...**
3. Enter profile name with date
4. Example: `Calibration_2024_07_22_Office_Lighting`
5. Add notes about conditions

### Load Calibration Profile

1. Open **Calibration > Load Profile**
2. Select calibration from list
3. Software loads all settings
4. Apply when conditions match

### Calibration History

**View Calibration Log:**
- Settings > Calibration > History
- Shows all calibrations performed
- Date, time, location, conditions
- Results and accuracy metrics
- Ability to revert to previous calibration

## Troubleshooting Calibration

### Common Issues

**"Calibration Failed" Message:**
- Ensure reference card properly positioned
- Check for shadows on card
- Verify lighting is stable
- Try again in different location
- Clean camera lens

**Poor Color Accuracy After Calibration:**
- Lighting may have changed
- Perform new calibration
- Verify reference card is white
- Check ColorChecker for damage

**Depth Accuracy Errors:**
- Ensure calibration plate is level
- Verify distance measurements
- Perform multi-point calibration
- Check plate for damage or warping

**Inconsistent Results:**
- Allow longer warm-up time
- Stabilize room temperature
- Perform thermal calibration
- Reduce environmental vibration

## Best Practices

1. **Calibrate on Installation** - Perform full calibration before first use
2. **Consistent Lighting** - Calibrate in typical working conditions
3. **Document Environment** - Note temperature, lighting, location
4. **Regular Validation** - Check accuracy weekly
5. **Multiple Profiles** - Create profiles for different lighting conditions
6. **Archive Results** - Keep historical calibration data
7. **Clean Lens** - Clean optics before calibration
8. **Stable Setup** - Use rigid mounting during calibration

## See Also

- [Operating Guide](./operating-guide.md)
- [Image Capture Settings](./image-capture-settings.md)
- [Technical Specifications](./technical-specifications.md)
