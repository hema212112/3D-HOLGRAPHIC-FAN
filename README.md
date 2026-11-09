# 3D Holographic Fan Display System

A group academic project exploring a rotating LED display that uses **Persistence of Vision (POV)** to create the appearance of images floating in mid-air.

## Project Overview

Conventional displays present images on flat screens. A POV-based holographic fan takes a different approach: LEDs mounted on a rotating assembly switch on and off at precisely timed intervals. Due to persistence of vision, the repeated light patterns are perceived as a complete image.

The project brings together embedded control, LED driving, motor rotation, timing synchronization, and image-to-POV mapping.

## Problem Statement

Flat displays require a physical screen and do not create the same floating-image effect. A rotating LED display can provide a compact visual alternative, but it requires accurate timing, stable rotation, reliable LED control, and safe mechanical construction.

## Objectives

- Explore a POV-based method for displaying floating visual content.
- Coordinate LED activation with the rotating assembly.
- Understand image preprocessing and radial LED mapping.
- Integrate the controller, LED driver, motor, and power circuitry.
- Evaluate visual clarity, flicker, alignment, and mechanical stability.

## Working Principle

1. **Prepare visual content:** Select an image, logo, text, or animation.
2. **Map the image:** Convert image data into radial display information suitable for a rotating LED array.
3. **Monitor rotation:** Use rotation feedback to estimate the rotor position and speed.
4. **Control LED timing:** Trigger LED patterns at the corresponding angular positions.
5. **Create the visual effect:** The eye combines the rapidly repeated light patterns into a continuous image.

## System Architecture

```text
Image / Animation
       |
       v
Image preprocessing and POV mapping
       |
       v
Microcontroller and timing logic <--- Rotation feedback
       |
       v
LED driver circuit
       |
       v
Rotating LED array ---> POV visual output

Motor and power stage ---> Rotational motion
```

## Hardware Blocks Described in the Report

- Arduino Uno microcontroller
- LED array / LED strip mounted on a rotating blade
- DC motor / high-speed motor assembly
- MOSFET-based LED driver
- Rotation feedback sensor (Hall-effect sensing is discussed in the implementation)
- Regulated power supply
- Mechanical support, mounting, and protective enclosure

**Configuration note:** The report describes different motor and power arrangements in its requirements and implementation sections. The final bill of materials should be updated only after checking the actual prototype.

## Software and Engineering Concepts

- Arduino IDE and Embedded C
- Timer-based LED triggering
- PWM motor-speed control
- Rotation-speed monitoring and timing adjustment
- Image preprocessing
- Cartesian-to-polar coordinate conversion
- Radial frame slicing and LED-position mapping

The report also discusses Python-based image processing. The corresponding source files are not currently available in this repository.

## Testing and Reported Observations

The report describes evaluation of:

- LED brightness and image clarity
- Flicker and frame alignment
- Motor speed and rotational stability
- Vibration and mechanical balance
- Power consumption and thermal behaviour

It reports that the prototype displayed logos, symbols, text animations, and simple motion graphics. An operating range of approximately **1200–1500 RPM** is reported for trials. These are observations stated in the project report, not independently reproduced measurements in this repository.

## Applications

- Retail advertising and product displays
- Exhibitions and events
- Educational demonstrations
- Museums and interactive installations
- Corporate and public information displays

## Possible Future Improvements

- Increase LED density for improved display resolution.
- Improve rotor balancing and vibration reduction.
- Enhance thermal management and enclosure design.
- Support easier content updates.
- Explore synchronization of multiple display units.
- Improve image conversion and animation preparation.

## Repository Structure

```text
3D-Holographic-Fan-Portfolio/
├── README.md
├── src/
│   └── README.md
├── hardware/
│   └── README.md
├── media/
│   └── README.md
└── docs/
    └── README.md
```



Author :

Hema A

Electronics and Communication Engineering — CMR Institute of Technology, Bengaluru.
