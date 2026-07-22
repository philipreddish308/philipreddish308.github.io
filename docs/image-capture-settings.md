# Image Capture Settings

## Resolution and Format

### Resolution Options

**Full Resolution:**
- **2048 × 1536 pixels**
- 24-bit RGB color
- File size: ~9-12 MB (uncompressed)
- Frame rate: Up to 30 fps
- Best for: High-quality inspections, archive

**Medium Resolution:**
- **1024 × 768 pixels**
- 24-bit RGB color
- File size: ~2-3 MB (uncompressed)
- Frame rate: Up to 60 fps
- Best for: Real-time monitoring, quick review

**Low Resolution:**
- **640 × 480 pixels**
- 24-bit RGB color
- File size: ~1 MB (uncompressed)
- Frame rate: Up to 120 fps
- Best for: Preview, network transmission

### File Formats

**JPEG (Lossy Compression)**
- Quality range: 60-100%
- File size: 25-40% of TIFF
- Best for: Web sharing, archive
- Loss: Minimal at 90%+

**PNG (Lossless Compression)**
- Full color information preserved
- File size: 40-60% of TIFF
- Best for: Quality with compression
- No quality loss

**TIFF (Uncompressed/Lossless)**
- Full resolution maintained
- File size: Maximum
- Best for: Professional work, archival
- No data loss

**BAYER RAW**
- Raw sensor data
- File size: ~6 MB per frame
- Best for: Advanced processing, research
- Requires post-processing

## Color Settings

### Color Space Selection

**sRGB (Default)**
- Standard for web and printing
- Gamma: 2.2
- Color gamut: 99% sRGB
- Best for: General use

**Adobe RGB**
- Extended color gamut
- Gamma: 2.2
- Color gamut: 62% of Adobe RGB
- Best for: Professional photography

**ProPhoto RGB**
- Widest gamut
- Gamma: 1.8
- Color gamut: 90% of ProPhoto
- Best for: High-end print work

### Color Profile Management

1. Open **Settings > Color**
2. Select color space from dropdown
3. Enable **ICC Profile** if needed
4. Load custom profile if available
5. Apply to live view and captures

### White Balance

**Automatic White Balance (AWB):**
- Default mode
- Analyzes entire frame
- Updates continuously in live view
- Best for: General use

**Preset Values:**

| Mode | Color Temp | Use Case |
|------|-----------|----------|
| Daylight | 5500K | Sunny conditions |
| Cloudy | 6500K | Overcast sky |
| Tungsten | 3200K | Incandescent lights |
| Fluorescent | 4500K | Fluorescent lights |
| Custom | User defined | Mixed lighting |

**Manual White Balance:**
1. Place white reference in scene
2. Click **Set White Balance**
3. Click on white surface
4. System calculates color correction
5. Apply to all future captures

### Saturation Control

**Range: 0-200%**
- 100% = Normal saturation
- <100% = Desaturated (toward grayscale)
- >100% = Oversaturated (vivid colors)
- Recommended: 90-110% for accurate colors

## Exposure Control

### Automatic Exposure (AE)

**AE Modes:**

**Matrix Metering:**
- Evaluates entire frame
- Balanced exposure
- Best for: Most subjects

**Center-Weighted:**
- Emphasizes center region
- Ignores bright surroundings
- Best for: Backlit subjects

**Spot Metering:**
- Uses single point (3-5% of frame)
- Precise control
- Best for: Small subjects

### Manual Exposure

**Shutter Speed:**
- Range: 1/4000 to 1 second
- Faster speed: Less blur, darker image
- Slower speed: More blur, brighter image

**ISO Sensitivity:**
- Range: 100 - 3200
- Lower ISO: Less noise, needs more light
- Higher ISO: More noise, works in dim light

**Recommended Combinations:**

| Lighting | Shutter | ISO | Notes |
|----------|---------|-----|-------|
| Bright sun | 1/4000 | 100 | Maximum speed |
| Overcast | 1/500 | 100 | Balanced |
| Indoor | 1/60 | 400 | Steady hand |
| Low light | 1/30 | 1600 | Use tripod |
| Dim | Bulb | 3200 | Manual focus |

### Exposure Compensation

**Range: -2.0 to +2.0 EV**

- -2.0 EV: 1/4 brightness
- -1.0 EV: 1/2 brightness
- 0.0 EV: Normal exposure
- +1.0 EV: 2× brightness
- +2.0 EV: 4× brightness

**Adjustment increments:**
- 1/3 EV (recommended)
- 1/2 EV
- 1 EV

## Focus Settings

### Autofocus Modes

**Continuous AF:**
- Camera continuously updates focus
- Follows subject movement
- Best for: Moving subjects
- Slower response than single AF

**Single AF:**
- Focus locks on trigger
- No tracking of movement
- Best for: Still subjects
- Faster response

**Manual Focus:**
- User sets focus distance
- No automatic adjustment
- Best for: Precise control
- Use focus distance slider

### Focus Distance Range

- **Minimum Focus:** 0.3m (11.8 inches)
- **Maximum Focus:** ∞ (infinity)
- **Hyperfocal Distance:** ~2m at f/2.8

### Focus Peaking

**Enable Focus Peaking:**
1. Settings > Focus > Enable Peaking
2. In-focus areas highlighted in color
3. Red: Sharp focus
4. Green: Acceptable focus
5. Blue: Out of focus

## Depth and 3D Settings

### Depth Map Quality

**Fast Mode:**
- Processing time: <50ms
- Real-time capture
- Lower accuracy: ±2mm
- Best for: Live preview

**Balanced Mode:**
- Processing time: ~100ms
- Good balance
- Accuracy: ±1.5mm
- Best for: Standard use

**High Quality Mode:**
- Processing time: ~200ms
- Best accuracy: ±0.5mm
- Requires post-processing
- Best for: Critical measurements

### Point Cloud Settings

**Point Cloud Format:**
- PLY (Polygon File Format)
- XYZ (ASCII coordinates)
- PCD (Point Cloud Data)

**Filtering Options:**
- Remove invalid points
- Voxel downsampling
- Statistical outlier removal

## Advanced Capture Options

### HDR (High Dynamic Range)

**Enable HDR:**
1. Settings > Advanced > Enable HDR
2. Capture multiple exposures
3. Combine into single image
4. Preserves highlights and shadows

**Tone Mapping:**
- Reinhard: Natural looking
- Drago: High contrast
- Mantiuk: Detail enhancement

### Bracketing

**Exposure Bracketing:**
- Captures 3-5 exposures at different levels
- Used for HDR or panorama
- Spacing: 1-2 EV recommended

**White Balance Bracketing:**
- Captures at different color temperatures
- Useful for mixed lighting

### Image Stabilization

**Electronic Stabilization:**
- Compensates for camera shake
- Slight field of view reduction
- Effective for: 1-2 stops

**Best Practices:**
- Use tripod for critical work
- Enable for handheld capture
- Combines with fast shutter speed

## Batch Processing

### Batch Capture Settings

1. Configure all capture parameters
2. Open **Batch > New Batch**
3. Define batch properties:
   - Number of images
   - Time interval
   - Save location
   - Naming convention
4. Click **Start Batch**
5. Monitor progress

### Naming Convention

**Variables Available:**
- {DATE} - Current date (YYYYMMDD)
- {TIME} - Current time (HHMMSS)
- {INDEX} - Sequential number
- {CUSTOM} - User defined text

**Example:** `IMG_{DATE}_{INDEX}.jpg`

## Profile Saving and Loading

### Save Capture Profile

1. Configure all desired settings
2. Click **Settings > Save Profile**
3. Enter profile name
4. Choose save location
5. Click **Save**

### Load Capture Profile

1. Click **Profile** dropdown menu
2. Select desired profile
3. All settings applied instantly
4. Ready to capture

### Built-in Profiles

- **Standard**: Balanced settings
- **High Quality**: Maximum resolution and quality
- **Fast**: Optimized for speed
- **Low Light**: Higher ISO and slower shutter
- **Studio**: Consistent professional settings

## Histogram and Exposure Preview

### Histogram Display

**Show Histogram:**
1. View > Show Histogram
2. RGB histogram shows color distribution
3. Adjust exposure to optimize

**Reading the Histogram:**
- Left edge: Black levels
- Center: Midtones
- Right edge: Highlights
- Clipping indicators show over/underexposure

### Live Exposure Preview

- Real-time feedback during adjustment
- Zebra stripes highlight blown highlights
- Blue areas indicate shadow clipping

## See Also

- [Operating Guide](./operating-guide.md)
- [Calibration Procedures](./calibration.md)
- [Technical Specifications](./technical-specifications.md)
