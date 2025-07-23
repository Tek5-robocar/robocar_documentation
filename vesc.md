---
layout: three-column
title: VESC Calibration
permalink: /vesc-calibration/
---

# Robocar: VESC Calibration

**An educational and research-ready platform for autonomous navigation**

## Introduction {#introduction}

The VESC (Vedder Electronic Speed Controller) is an open-source motor controller for electric vehicles and robotics. Calibration ensures accurate sensor readings, smooth motor performance, and system optimization.

## Required Tools and Software {#tools}

- VESC included in your kit  
- Micro-USB cable  
- Computer (Windows, macOS, or Linux)  
- [VESC Tool](https://vesc-project.com/)

## Configuration {#configuration}

### A. Hardware Setup {#hardware-setup}

1. **Power Connection**  
   Connect the VESC to the 4S LiPo battery using an XT60 (or compatible) connector. Ensure correct polarity.

2. **Motor Connection**  
   Connect the three wires of the BLDC motor to the VESC. The order doesn't matter initially.

3. **Servo Motor Connection**  
   Plug the servo motor into the PWM output port of the VESC.

4. **USB Connection**  
   Connect the VESC to your laptop via USB.

**Diagram:**  
![Hardware Setup](./images/vesc_calibration_electric_diagram.png)

---

### B. VESC Tool Setup {#vesc-tool-setup}

1. **Open the VESC Tool**  
   Launch the application and accept the terms and conditions.

   ![VESC Tool Home](path/to/vesc-tool-home.png)

2. **Connect to VESC Device**  
   Select your VESC from the list. Linux users may need to add themselves to the `dialout` group.

   ![VESC Connect](path/to/vesc-connect.png)

3. **Firmware Update** (optional)  
   If prompted, update the firmware using the Firmware Manager.

   ![Firmware Manager](path/to/firmware-manager.png)  
   ![Firmware Upload](path/to/firmware-confirmation.png)

4. **Motor Setup**  
   Reconnect the VESC, then go to motor setup:

   - Select the third option
   - Fill in battery information
   - Confirm the configuration

   ![Battery Info](path/to/battery-info.png)

   - Enter motor specifications  
   - Ensure wheels are elevated on a stand  

   ![Motor Info](path/to/motor-info.png)

   - After motor spins, confirm success

   ![Motor Success](path/to/motor-success.png)

   - Go to **Motor Settings > General**, switch from FOC to **BLDC**
   - Save configuration

   ![Write Configuration](path/to/write-configuration.png)

---

## Motor Test {#motor-test}

You can test the motor by pressing the motor test button and using the arrow keys on your keyboard.

![Motor Test](path/to/motor-test.png)

---

## Servo Setup {#servo-setup}

- Go to **App Settings > General**
- Enable **Servo Output**
- Save and go to the test tab

![Servo Setup](path/to/servo-setup.png)  
![Servo Test](path/to/servo-test.png)

---

## Notes {#notes}

- Always place the car on a stand before spinning the motor
- Double-check all power and motor connections before operation
- If using Linux, ensure USB permissions are set correctly (`dialout` group)

&nbsp;

To report problems or suggest improvements to this calibration guide, open an issue or submit a pull request in the corresponding Git repository. Please include any screenshots or log outputs when applicable to ensure effective troubleshooting and updates.
