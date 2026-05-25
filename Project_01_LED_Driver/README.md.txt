# Project 01 — LED Driver PCB (V2)

## Overview

This is my first PCB design project created completely from scratch using KiCad.

The project is a simple transistor-based LED driver circuit using a PN2222A NPN transistor as a low-side switch. Even though the circuit itself is simple, the main goal of this project was to deeply understand PCB fundamentals instead of blindly following tutorials.

This project helped me learn:
- Schematic design
- Datasheet reading
- PCB layout workflow
- ERC and DRC debugging
- Ground planes / copper pours
- Routing strategy
- Current flow and return paths
- Silkscreen and manufacturability considerations

---

# Circuit Description

The circuit uses:
- PN2222A NPN transistor
- Current limiting resistor for LED
- Base resistor for transistor switching
- Push button switch
- 12V input supply
- Single LED load

The transistor works as a low-side switch:
- Pressing the switch provides base current
- The transistor saturates
- The LED turns ON

---

# Why I Chose a Simple Circuit

I intentionally chose a simple transistor LED driver because I wanted to focus on:
- Understanding how current actually flows
- Why each component exists
- PCB placement and routing fundamentals
- Grounding concepts
- Physical implementation of schematics

Instead of jumping directly into MCU or complex boards.

---

# Design Calculations

## LED Resistor

Using:
- Supply Voltage = 12V
- LED Forward Voltage ≈ 2V
- LED Current ≈ 20mA

Calculation:

R = (12V - 2V) / 0.02A = 500Ω

Standard value used:
- 560Ω

---

## Transistor Base Resistor

Using forced beta saturation approach:

- Collector current ≈ 20mA
- Forced beta ≈ 10

Required base current:

Ib = 20mA / 10 = 2mA

Base resistor:

Rb = (12V - 0.7V) / 0.002A ≈ 5.6kΩ

---

# V1 → V2 Improvements

After receiving community feedback and reviewing the PCB again, I redesigned the board into Version 2.

Improvements made:
- Added proper GND copper pour
- Improved current return paths
- Reduced unnecessary routing detours
- Improved component placement
- Added mounting holes
- Added silkscreen labels
- Added board versioning
- Improved routing consistency
- Fixed ERC/DRC issues
- Learned thermal relief behavior
- Improved PCB readability and organization

---

# Tools Used

- KiCad 10
- Git & GitHub
- Datasheets
- Google research
- Engineering community feedback

---

# What I Learned

This project taught me that PCB design is not just drawing lines between components.

It involves:
- Electrical behavior
- Physical geometry
- Current return paths
- Manufacturability
- Mechanical constraints
- Debugging workflow

One of the biggest lessons was understanding that:
> Schematic defines electrical intent, PCB defines physical implementation.

---

# Future Improvements

Future versions may include:
- MOSFET-based switching
- MCU control input
- Reverse polarity protection
- Proper connector selection
- 2-layer optimized routing
- Decoupling capacitors
- Compact PCB optimization

---

# Repository Structure

```text
Project_01_LED_Driver/
├── PCB/
├── Schematics/
├── Gerbers/
├── Images/
├── Datasheets/
└── README.md
```

---

# Status

Completed — Beginner PCB Project V2