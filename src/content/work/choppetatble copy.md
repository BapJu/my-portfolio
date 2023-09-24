---
title: Virtual Thermal Exchange Test Bench for Homes
publishDate: 2023-05-02 00:00:00
img: /assets/Virtual_Thermal_Exchange.png
img_alt: Picture of a raspberry pi and a NFC reader
description: |
  Creation of a test bench to virtually model the thermal exchange of a house, spanning multiple academic disciplines.
tags:
  - Analog Electronics
  - Microcontroller (STM32)
  - C language
---
## Overview

The project involved the construction of a "virtual" version that incorporated different modules developed during various educational projects:

1. **Embedded software** for acquisition & control developed during the "Digital Electronics on Microcontroller (ELN STM32)" project.
2. **Embedded software** for supervision & temperature regulation developed during the "Informatics" project.
3. **Electronical module** for simulating thermal exchange in a dwelling was crafted during the "Analog Electronics (ELA)" project.

## Key Features

### 1. Thermal Exchange Simulator

- Purely electronic module using RC models to mimic the thermal exchange of a dwelling.
- Can simulate opening or closing of a window.
- Capable of modeling temperatures ranging from 0°C to 50°C.
- Utilizes a time-scale change for faster simulation: 4ms simulation period equates to a real-world period of 10s.
- Exterior temperature is adjustable via a potentiometer, allowing for the simulation of daily temperature variations.
- Temperatures are digitized using an AD7991-0 converter from ANALOG DEVICES with I2C connectivity.
- Heating is controlled using PWM (Pulse Width Modulation).

### 2. Acquisition & Control Interface Module

- Core component is an STM32L152 microcontroller.
- Capable of programming practical work.
- Receives temperature measurements digitally via I2C.
- Computes and displays internal and external temperatures.
- Receives heating control commands from the temperature regulation module via USB.
- Features an interface consisting of:
  - 8 LEDs
  - A 128 x 160 pixel color screen
  - A potentiometer
  - 3 push buttons

### 3. Supervision & Temperature Regulation Module

- Executed via PC software.
- Responsibilities include:
  - Managing internal temperature settings.
  - Regulating internal temperature.
  - Controlling heating.
  - Recording temperatures and commands.

## Significance

This multidisciplinary project serves as a practical tool for understanding and simulating the complexities of thermal exchanges in buildings. It combines electronics, embedded systems, and computer-based supervision, providing a comprehensive platform for academic exploration and innovation.