# Capstone Project: Integrated Power Electronics & Embedded Systems

This repository contains the design, simulation, firmware, and implementation files for my ongoing engineering Capstone Project. The project bridges heavy hardware design (custom magnetics and switching topologies) with precision analog front-ends and real-time digital signal processing (DSP) to create an optimized, closed-loop embedded power system.

## Project Metadata
* **Author:** Aarav Balaji (B.Tech EEE, NITK Surathkal '28)[cite: 5]
* **Timeline:** September 2025 – Ongoing[cite: 5]
* **Academic Advisor:** Prof. Prajof Prabhakaran (Department of EEE, NITK)[cite: 5]
* **Department:** Electronics & Electrical Engineering Department, NITK[cite: 5]

---

## Technical Architecture & Core Pillars

The project is executed across three interdependent engineering disciplines:

### 1. Magnetics & Power Hardware Design
Focused on the core mathematical sizing, optimization, and physical fabrication of passive components for robust power delivery platforms[cite: 5].
* **Topologies Implemented:** Linear Regulated Power Supplies and Buck Converter switching topologies[cite: 5].
* **Custom Core Calculations:** Performed analytical modeling for inductor and capacitor sizing to bound voltage/current ripple under specific transient profiles.
  * *Inductor Sizing Formula:* 
    $$L = \frac{V_{\text{in}} - V_{\text{out}}}{\Delta I_L} \cdot \frac{D}{f_s}$$
* **Fabrication:** Hand-wound custom magnetic cores and assembled power stages to withstand targeted current loads without saturating[cite: 5].

### 2. Analog Signal Conditioning
Designed high-precision analog front-ends (AFEs) to interface high-power rails with sensitive low-voltage microcontrollers safely and accurately[cite: 5].
* **Topology:** Optimized Operational Amplifier (Op-Amp) and Instrumentation Amplifier configurations[cite: 5].
* **Functionality:** Implemented precise active filtering, scaling, and level-shifting to maximize the dynamic range of the microcontroller's Analog-to-Digital Converter (ADC) while isolating high-frequency switching noise[cite: 5].

### 3. Digital Signal Processing (DSP) & Embedded Control
Developed real-time firmware architecture to process conditioned sensor data and maintain closed-loop system stability[cite: 5].
* **Modeling:** Built discrete-time software representations and mathematically modeled digital filter coefficients using MATLAB to analyze frequency and phase responses[cite: 5].
* **Implementation:** Deployed high-speed execution loops on embedded platforms (Arduino/ESP32) utilizing real-time DSP algorithms to regulate power loops dynamically[cite: 5].

---

## Tech Stack & Toolchain

| Category | Tools & Technologies |
| --- | --- |
| **Simulation & Modeling** | LTspice, MATLAB, Simulink[cite: 5] |
| **Hardware Design** | KiCad, Custom Magnetics Core Calculators, PCB Design[cite: 5] |
| **Embedded Programming** | C, C++, Arduino IDE, ESP32 Architecture[cite: 5] |

---

## Current Status & Ongoing Work
Because this is an actively evolving project, development is tracking through the following milestones[cite: 5]:
* [x] Mathematical modeling of custom magnetic components and open-loop hardware verification[cite: 5].
* [x] MATLAB simulation of digital filter topologies and frequency response verification[cite: 5].
* [ ] Hardware-in-the-loop (HIL) testing combining the analog front-end with real-time DSP firmware routines.
* [ ] Final multi-layer PCB layout routing and structural containment design.

---

## References & Documentation
* Documentation and hardware calculation sheets can be found in the `/magnetics` and `/hardware` directories.
* Standard reference texts utilized: Ned Mohan, *Power Electronics: Converters, Applications, and Design*.
