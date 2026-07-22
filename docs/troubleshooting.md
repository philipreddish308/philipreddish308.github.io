# Troubleshooting Guide

## Connection Issues

### Camera Not Detected

**Problem:** Camera appears in Device Manager but not in software

**Solutions:**

1. **Verify USB Connection**
   - Try different USB 3.0 port
   - Use primary USB port (not hub)
   - Check cable for damage
   - Replace with new USB 3.0 cable

2. **Reinstall Drivers**
   - Windows:
     - Open Device Manager
     - Right-click camera device
     - Select "Uninstall device"
     - Restart computer
     - Reconnect camera
   - macOS:
     - System Preferences > Security & Privacy
     - Allow camera driver installation
     - Reconnect camera

3. **Update Software**
   - Check for software updates
   - Install latest version
   - Restart computer
   - Reconnect camera

4. **Check USB Hub**
   - Disconnect any USB hubs
   - Connect directly to computer
   - Test with different ports

### USB Connection Drops

**Problem:** Camera disconnects randomly during operation

**Solutions:**

1. **Cable Issues**
   - Inspect cable for damage
   - Test with different cable
   - Secure cable connection
   - Avoid cable strain

2. **Power Supply**
   - Use dedicated 5V/2A power adapter
   - Avoid USB bus power for extended use
   - Check power connector for corrosion
   - Replace power cable if damaged

3. **Thermal Issues**
   - Allow camera to cool (stop operation for 5 minutes)
   - Improve ventilation around camera
   - Check for blocked cooling vents
   - Reduce continuous operation time

4. **USB Controller Issues**
   - Update USB controller drivers
   - Disable USB Selective Suspend:
     - Power Options > Change plan settings > Change advanced power settings
     - USB settings > USB selective suspend setting > Disabled

## Software Issues

### Software Won't Start

**Problem:** Application crashes or fails to launch

**Solutions:**

1. **Verify System Requirements**
   - Check OS version
   - Confirm RAM available (>4GB free)
   - Ensure disk space (>1GB free)
   - Update graphics drivers

2. **Repair Installation**
   - Windows: Programs > Programs and Features > RobotAI Camera > Repair
   - macOS: Drag RobotAI Camera to Trash > Empty Trash > Reinstall

3. **Clean Installation**
   - Completely uninstall software
   - Restart computer
   - Download fresh installer
   - Install to default location
   - Run as Administrator (Windows)

4. **Dependency Check**
   - Verify .NET Framework installed (Windows)
   - Update Visual C++ Runtime
   - Install latest DirectX (Windows)
   - Check GPU drivers are current

### Software Crashes

**Problem:** Application crashes during operation

**Solutions:**

1. **Check Error Log**
   - Help > View Error Log
   - Note error code and message
   - Check timestamp

2. **Memory Issues**
   - Close unnecessary applications
   - Reduce resolution
   - Disable advanced features
   - Check available RAM

3. **GPU Issues**
   - Update graphics drivers
   - Disable GPU acceleration:
     - Settings > Advanced > Disable GPU Acceleration
   - Test with different GPU (if available)

4. **File Corruption**
   - Delete configuration files
   - Uninstall completely
   - Install fresh copy
   - Run repair utility

## Image Quality Issues

### Blurry Images

**Problem:** Captured images are out of focus

**Solutions:**

1. **Focus Issues**
   - Verify autofocus is working
   - Check focus distance (300mm minimum)
   - Enable focus peaking to verify focus
   - Manually adjust focus slider
   - Clean camera lens

2. **Motion Blur**
   - Increase shutter speed
   - Use tripod or stabilization
   - Increase lighting level
   - Enable image stabilization

3. **Depth of Field**
   - Subject may be outside focus range
   - Move closer to subject
   - Adjust focus distance slider
   - Verify working distance

### Dark or Underexposed Images

**Problem:** Images are too dark

**Solutions:**

1. **Check Lighting**
   - Improve room lighting
   - Add supplemental lighting
   - Reposition light sources
   - Reduce shadows

2. **Adjust Exposure**
   - Increase exposure compensation (+0.5 to +2.0 EV)
   - Increase ISO (100-3200)
   - Decrease shutter speed
   - Enable auto exposure

3. **Power Check**
   - Verify camera powered
   - Check LED indicator
   - Confirm external power connected
   - Test with different power supply

### Overexposed Images (Blown Highlights)

**Problem:** Images are too bright or washed out

**Solutions:**

1. **Reduce Exposure**
   - Decrease exposure compensation (-2.0 to -0.5 EV)
   - Reduce ISO to 100
   - Increase shutter speed (faster)
   - Enable auto exposure

2. **Lighting Adjustment**
   - Reduce light intensity
   - Reposition light sources
   - Use diffusers
   - Move away from bright light

3. **Check Metering**
   - Switch metering mode (spot, center-weighted)
   - Adjust exposure based on histogram
   - Enable exposure preview

### Color Issues

**Problem:** Colors appear inaccurate or incorrect

**Solutions:**

1. **White Balance**
   - Recalibrate white balance
   - Use white balance reference card
   - Verify lighting color temperature
   - Select appropriate white balance preset

2. **Color Profile**
   - Select correct color space (sRGB default)
   - Load appropriate ICC profile
   - Verify display color calibration
   - Test on different display

3. **Lighting Change**
   - Colors may shift with different lighting
   - Recalibrate for new lighting conditions
   - Use consistent lighting setup
   - Document lighting conditions

## Performance Issues

### Slow Frame Rate

**Problem:** Camera captures fewer frames than expected

**Solutions:**

1. **Check System Load**
   - Close unnecessary applications
   - Monitor CPU usage (should be <80%)
   - Monitor RAM usage
   - Check disk I/O activity

2. **Reduce Processing Load**
   - Lower resolution (1024×768)
   - Disable depth processing
   - Disable real-time preview
   - Use faster image format (JPEG)

3. **Optimize Settings**
   - Reduce image quality
   - Disable advanced features
   - Use High-Speed mode
   - Enable GPU acceleration

4. **Storage Issues**
   - Write to faster storage (SSD)
   - Free up disk space (>10GB recommended)
   - Check file system (defragment if needed)
   - Move working directory to faster drive

### High CPU Usage

**Problem:** Computer CPU usage is very high

**Solutions:**

1. **Reduce Processing**
   - Lower resolution
   - Disable real-time features
   - Turn off depth processing
   - Disable preview

2. **Disable Advanced Features**
   - Settings > Advanced > Disable
   - Disable GPU acceleration testing
   - Reduce color processing
   - Disable histogram updates

3. **Close Background Tasks**
   - Close other applications
   - Disable cloud sync temporarily
   - Stop antivirus scanning
   - Disable screensaver effects

### Memory Leaks

**Problem:** Memory usage increases over time

**Solutions:**

1. **Restart Application**
   - Close RobotAI Camera software
   - Wait 10 seconds
   - Reopen application
   - Memory should reset

2. **Reduce Capture Time**
   - Avoid continuous operation >2 hours
   - Take breaks between capture sessions
   - Restart software periodically
   - Monitor memory in Task Manager

3. **Check File System**
   - Reduce number of open files
   - Archive old images
   - Clear temporary files
   - Restart computer

## Thermal Issues

### Overheating Warning

**Problem:** LED shows yellow, thermal warning appears

**Solutions:**

1. **Cool Down Camera**
   - Stop operation immediately
   - Allow 10-15 minutes cool-down time
   - Ensure cooling vents not blocked
   - Improve ambient ventilation

2. **Reduce Usage**
   - Lower frame rate
   - Reduce resolution
   - Disable advanced features
   - Take breaks between captures

3. **Environmental**
   - Reduce room temperature
   - Improve air circulation
   - Move camera away from heat sources
   - Use cooling fan nearby (not direct)

## Power Issues

### Low Power Warning

**Problem:** LED shows yellow, low power message

**Solutions:**

1. **Check Power Supply**
   - Verify 5V/2A adapter connected
   - Check power cable connection
   - Test power adapter with voltmeter
   - Replace if damaged

2. **Use External Power**
   - Connect external power adapter
   - Do not rely on USB bus power alone
   - Ensure dedicated power supply
   - Use quality power adapter

3. **Check Power Connector**
   - Inspect connector for corrosion
   - Clean connector carefully
   - Verify firm connection
   - Test with different cable

## Depth/3D Issues

### Depth Map Not Available

**Problem:** Depth processing fails or returns no data

**Solutions:**

1. **Verify Sensor**
   - Check camera LED indicator
   - Restart software
   - Reconnect USB cable
   - Update firmware

2. **Enable Depth Processing**
   - Settings > Depth > Enable Depth Processing
   - Select quality level (Balanced recommended)
   - Apply settings
   - Capture new image

3. **Check Subject**
   - Subject must be within 300-1500mm
   - Ensure subject is visible
   - Avoid reflective surfaces
   - Adequate lighting required

### Noisy Depth Data

**Problem:** Depth map contains errors or noise

**Solutions:**

1. **Improve Lighting**
   - Increase ambient lighting
   - Avoid harsh shadows
   - Use diffused lighting
   - Ensure even illumination

2. **Adjust Distance**
   - Move closer to subject
   - Maintain 300-800mm optimal range
   - Verify subject size
   - Check focus

3. **Switch Quality Mode**
   - Use High Quality mode for better accuracy
   - Allow more processing time
   - Reduce frame rate
   - Verify results improve

## Calibration Issues

### Calibration Failed

**Problem:** Calibration process fails

**Solutions:**

1. **Check Reference Target**
   - Verify reference card not damaged
   - Ensure card is white and clean
   - Position card properly in frame
   - Avoid shadows on card

2. **Lighting Requirements**
   - Ensure even lighting
   - Avoid backlight
   - Stable lighting (no flicker)
   - Adequate brightness

3. **Positioning**
   - Position card perpendicular to camera
   - Fill most of frame
   - Keep camera steady
   - Use tripod for stability

4. **Try Again**
   - Clear any error messages
   - Move to different location
   - Try under different lighting
   - Restart software

## Contacting Support

If issues persist after troubleshooting:

1. **Collect Information**
   - Error messages and codes
   - Software version
   - Operating system version
   - USB device serial number
   - Recent changes or updates

2. **Prepare Documentation**
   - Screenshots of error
   - Error log file
   - System information
   - Steps to reproduce issue

3. **Contact Support**
   - Email: support@robotai.com
   - Phone: +1-555-ROBOT-AI
   - Website: www.robotai.com/support
   - Include all collected information

## See Also

- [Getting Started](./getting-started.md)
- [Operating Guide](./operating-guide.md)
- [Technical Specifications](./technical-specifications.md)
- [Support](./support.md)
