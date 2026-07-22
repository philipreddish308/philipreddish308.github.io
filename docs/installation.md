# Installation Guide

## System Requirements

### Minimum Requirements

- **Operating System:** Windows 10, macOS 10.14+, or Ubuntu 18.04 LTS
- **Processor:** Intel i5 (6th Gen) or equivalent
- **RAM:** 8GB
- **Storage:** 500MB available space
- **USB Port:** USB 3.0 or higher

### Recommended Specifications

- **Processor:** Intel i7 (8th Gen) or newer
- **RAM:** 16GB
- **Storage:** SSD with 2GB available space
- **USB Port:** Multiple USB 3.0 ports
- **Display:** 1920×1200 resolution or higher

## Software Installation

### Windows

1. Download the RobotAI Camera software from the website
2. Run `RobotAI_Camera_Setup.exe`
3. Accept the license agreement
4. Choose installation location (default: `C:\Program Files\RobotAI`)
5. Select components to install:
   - ✓ Core Software (required)
   - ✓ USB Drivers (required)
   - ☐ Development Tools (optional)
   - ☐ Sample Projects (optional)
6. Click **Install** and wait for completion
7. Restart your computer when prompted

### macOS

1. Download the RobotAI Camera package
2. Open `RobotAI_Camera.dmg`
3. Drag the RobotAI Camera icon to the Applications folder
4. Wait for the copy process to complete
5. Open Applications folder and double-click RobotAI Camera
6. Grant any requested permissions
7. Installation is complete

### Linux (Ubuntu)

```bash
# Add repository
sudo add-apt-repository ppa:robotai/camera
sudo apt-get update

# Install
sudo apt-get install robotai-camera

# Verify installation
robotai-camera --version
```

## Hardware Setup

### Physical Installation

1. **Locate Installation Space**
   - Choose a stable surface or mounting point
   - Ensure clearance around the camera
   - Avoid direct sunlight exposure

2. **Mount the Camera**
   - Attach to tripod or mounting bracket
   - Ensure secure connection
   - Use the included M4 mounting plate if needed

3. **Cable Management**
   - Connect USB 3.0 cable to computer
   - Connect power adapter to camera
   - Use cable clips to manage wire routing
   - Keep cables away from heat sources

### Environmental Considerations

- **Temperature:** Install in environment maintained at 15-30°C
- **Humidity:** Avoid areas with high humidity or condensation
- **Vibration:** Minimize vibrations from nearby equipment
- **Lighting:** Position to avoid direct sunlight on sensor

## Driver Installation

### Automatic Driver Installation

Most systems automatically install required USB drivers. To verify:

1. Connect the camera via USB
2. Wait 10-15 seconds
3. Check Device Manager (Windows) or System Report (macOS)
4. Camera should appear as "RobotAI Camera"

### Manual Driver Installation

If automatic installation fails:

**Windows:**
1. Download drivers from support website
2. Extract to a known location
3. Open Device Manager
4. Right-click unknown device
5. Select "Update driver"
6. Choose "Browse my computer for drivers"
7. Navigate to extracted folder
8. Complete installation

**macOS:**
1. Open System Preferences
2. Go to Security & Privacy
3. Allow installation of developer software
4. Reconnect camera

## First Connection Test

1. Open RobotAI Camera software
2. Go to **Settings > Device Manager**
3. Click **Scan for Devices**
4. Your camera should appear in the list
5. Select and click **Connect**
6. Status should show "Connected"

## Firmware Update

To update camera firmware:

1. Connect camera to computer
2. Open RobotAI Camera software
3. Go to **Settings > Firmware Update**
4. Click **Check for Updates**
5. If update available, click **Update**
6. Do not disconnect during update process
7. Camera will restart automatically

## Troubleshooting Installation

### Camera Not Detected

- Check USB cable connection
- Try different USB port (preferably 3.0)
- Restart the computer
- Verify drivers are installed
- Check System Information for device errors

### Software Won't Start

- Verify system requirements are met
- Check hard drive space (minimum 500MB)
- Disable antivirus temporarily
- Reinstall software
- Check compatibility mode settings

### Performance Issues

- Check CPU and RAM usage
- Close unnecessary applications
- Update GPU drivers
- Reduce resolution in settings
- Enable power-saving mode on USB hub

## Post-Installation

After successful installation:

1. Perform [Calibration](./calibration.md)
2. Review [Operating Guide](./operating-guide.md)
3. Explore [Image Capture Settings](./image-capture-settings.md)
4. Run sample projects included in installation

## See Also

- [System Requirements](./system-requirements.md)
- [Troubleshooting Guide](./troubleshooting.md)
- [Getting Started](./getting-started.md)
