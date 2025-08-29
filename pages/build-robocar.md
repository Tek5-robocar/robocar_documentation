---
layout: three-column
title: Build Robocar
permalink: /build-robocar/
description: Step-by-step guide to assembling the Robocar, from mechanical construction to electronics integration, including tips for wiring, mounting, and calibration.
---

## Tools Required

- Precision screwdriver set  
- Wire stripper  
- Soldering iron  
- Cutting pliers  
- Flat pliers  
- M3 tap (for threading 3 mm screw holes)

## Removing RC Control Components

Before building your Robocar, you must remove the original RC control system — typically the receiver and electronic speed controller (ESC) — to make space for the onboard AI electronics and motor controller (VESC).

**⚠️ Important:** Make sure the car is powered off and the battery is disconnected before starting.

### Step 1: Remove the Top Shell

1. Unscrew the four body clips that secure the plastic shell to the chassis.
2. Carefully lift the shell and set it aside. It will be reused.

### Step 2: Detach the Rear Wing and Mounts

1. Use a screwdriver to remove the rear wing and its plastic mounting brackets.
2. Keep the screws; some may be reused for mounting new components.

> Below is a photo of the car **with the plastic shell removed**, exposing the inner chassis:

<img src="./../images/car_building/car_without_body.jpg" alt="Chassis without body" width="400" style="max-height: 2500px; object-fit: contain; transform: rotate(180deg);"/>

### Step 3: Unplug and Remove the RC Receiver and ESC

1. Locate the RC receiver and the ESC (often mounted in plastic holders or boxes).
2. Carefully unplug all connectors: battery input, motor wires, and servo plug.
3. Unscrew or unclip the receiver and ESC from the chassis.
4. Set them aside. They will be replaced by the Jetson Nano and VESC modules.

> After removing these components, you should see an **empty central frame** like in the image below — ready to receive custom mounts and electronics:

<img src="./../images/car_building/car_empty.jpg" alt="Chassis without traxxas components" width="400" style="max-height: 2500px; object-fit: contain;"/>

## Install the VESC Module

Now that the original electronics have been removed, it's time to mount the VESC (motor controller) using its custom 3D-printed support.

1. Place the 3D-printed VESC support clip into the central area of the chassis, where the original ESC was located.

> Below is a photo of the car **with the 3D-printed VESC support installed**, ready to receive the controller:

<img src="./../images/car_building/car_with_vesc_support.jpg" 
     alt="VESC support mounted in chassis" 
     width="400" 
     style="max-height: 2500px; object-fit: contain;" />

2. Secure the support to the chassis using M3 screws or zip ties through the dedicated holes.

3. Carefully insert the VESC module into the 3D-printed clip until it clicks or fits snugly.

4. Plug the motor wires into the VESC (keep track of wire order for later calibration).

5. Leave the power input and servo signal cables accessible — they will be connected later to the Jetson Nano and power source.

> Below is a photo of the car **with the VESC mounted and fully connected** (motor, servo, and power wires visible):

<img src="./../images/car_building/car_vesc_connected.jpg" 
     alt="VESC connected" 
     width="400" 
     style="max-height: 2500px; object-fit: contain;" />

To continue, you now need to flash and configure the VESC for use with your Robocar.  
➡️ Please refer to the [VESC Setup section](../vesc-calibration/) for detailed instructions.
