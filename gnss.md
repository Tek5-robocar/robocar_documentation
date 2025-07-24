---
layout: three-column
title: GNSS RTK GPS - Point One
permalink: /gnss-rtk-gps/
---

# Robocar: GNSS RTK GPS Setup (Point One Standard Dev Kit)

**An educational and research-ready platform for autonomous navigation**

---

## 1. Introduction {#introduction}

The Point One Navigation Standard Development Kit provides real-time kinematic (RTK) positioning with centimeter-level accuracy. This GPS solution is designed for integration into autonomous systems such as robotic cars and drones. Proper setup and flashing ensure the device is recognized and ready for software integration and high-accuracy location tracking.

---

## 2. Requirements {#requirements}

To follow this tutorial, you will need:

- A Windows or macOS computer  
- The Point One Navigation Standard Dev Kit  
- A micro-USB cable (usually provided in the kit)  
- Internet access to download required drivers and tools

---

## 3. Flashing Tutorial {#flashing}

Follow these steps to set up your device correctly.

### A. Install USB Serial Driver {#install-driver}

To begin, install the USB serial driver so your computer can recognize the connected GNSS module.

- 👉 Download the driver from Point One Navigation’s documentation site:  
  [https://support.pointonenav.com](https://support.pointonenav.com)  
  *(Search for “USB Serial Driver” or visit the Standard Dev Kit documentation section.)*

- After installation, connect the Point One Dev Kit to your PC using a USB cable.

- Confirm the device is recognized by checking your:
  - **Device Manager** (Windows)  
  - **System Information > USB** (macOS)

**Screenshot Placeholder:**  
![Image](path/to/screenshot_device_recognition.png)

---

### B. Launch Flashing Utility {#flashing-utility}

<!-- Placeholder for next step: launching the flashing software -->
<!-- Add UI screenshots here once available -->

**Screenshot Placeholder:**  
![Image](path/to/screenshot_flashing_utility.png)

---

### C. Load Latest Firmware {#load-firmware}

<!-- Placeholder for firmware loading step -->

**Screenshot Placeholder:**  
![Image](path/to/screenshot_firmware_load.png)

---

### D. Confirm Flashing and Reboot {#confirm-flash}

<!-- Placeholder for successful flashing confirmation -->

**Screenshot Placeholder:**  
![Image](path/to/screenshot_flash_success.png)

---

## 4. Python Development {#python-dev}

*This section will describe how to interface with the Point One Navigation Dev Kit using Python (e.g. serial communication, parsing NMEA or custom messages, etc.).*

---

## ✅ Notes

- Ensure the device is on a flat, unobstructed surface when testing GPS lock.
- Some installations (especially on Windows) may require rebooting after driver installation.
- Avoid powering down the device during firmware flashing.

---

For issues or improvements, open a GitHub issue or submit a pull request. Please attach logs, error messages, or screenshots to help debug efficiently.
