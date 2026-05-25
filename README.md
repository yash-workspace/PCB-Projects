# My PCB Design Journey

Welcome! This repository is a living document of my hands-on journey into the world of PCB design and practical electronics using KiCad.

For me, this isn't just about connecting dots on a screen or getting an LED to blink. It’s about deeply understanding what happens beneath the surface—mastering current flow, grounding, return paths, routing strategies, and designing for actual manufacturability.

Instead of blindly copying tutorial schematics, I build these projects from the ground up using **datasheets, engineering research, messy experimentation, and iterative redesigns** based on real-world feedback.

---

# The Toolkit

* **Design:** KiCad 10
* **Version Control:** Git & GitHub (because breaking things is part of the process)
* **Validation:** Rigorous DRC/ERC workflows
* **Knowledge Base:** Deep-dives into datasheets & community code reviews

---

# Repository Structure

```text
PCB-Projects/
│
├── Project_01_LED_Driver/   # My gateway project (Transistor-based)
│
├── Project_02_...          # Incoming designs...
│
└── Future Projects/         # The roadmap

```

---

# The Projects

## Project 01 — LED Driver PCB (V2)

My gateway into hardware: a transistor-based LED driver utilizing a PN2222A transistor, a current-limiting resistor, a push-button switch, and a 12V input.

While the circuit itself is fundamental, the real challenge was transitioning from a breadboard mindset to a hardware manufacturing mindset. I used this project to cut my teeth on schematic capture, copper pours, proper grounding, and wrestling with DRC/ERC errors.

### The Evolution: V1 → V2

Design is iterative, and V1 had plenty of room for improvement. Here is what changed in the second revision:

* **Better Power Delivery:** Added a dedicated GND copper pour and optimized current return paths.
* **Cleaner Routing:** Overhauled the trace strategy for cleaner signal flow and better organization.
* **Mechanical Basics:** Added mounting holes and clear, legible silkscreen labels for easier debugging.
* **Production Ready:** Fixed lingering DRC/ERC issues to ensure the board can actually be fabricated.

 **Explore the project files:** Check out the `Project_01_LED_Driver/` folder.

---

# What I’m Chasing Next

### Current Focus

* Solidifying PCB layout fundamentals
* Mastering datasheet-driven design
* Developing a reliable hardware debugging workflow
* Bridging the gap between embedded systems and physical hardware

### On the Horizon

* Moving to MOSFET switching and complex power electronics
* Stepping up to dense 2-layer (and eventually multi-layer) designs
* Designing custom microcontroller (MCU) boards and sensor interfaces
* Robotics electronics

---

# A Key Lesson So Far

If there is one major takeaway I've had so far, it’s this:

> **Schematics define electrical intent. PCB layout defines physical electromagnetic implementation.**

Even the simplest 12V circuit forces you to balance electrical engineering, mechanical constraints, and the physics of how current actually behaves on copper.

---

# Project Status

**Actively building, breaking, and iterating.** Feel free to look around, check out the schematics, or drop some feedback if you see room for improvement!
