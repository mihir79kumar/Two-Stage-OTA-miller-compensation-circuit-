# Design and Analysis of Two-Stage CMOS Operational Amplifier using eSim

## Overview  
This project presents the design and analysis of a **two-stage CMOS operational amplifier** implemented using **eSim** and **Ngspice** at a **1.8 V** supply voltage.  
The amplifier ensures all MOSFETs operate in the saturation region to achieve **high gain**, **good stability**, and **wide bandwidth**.

---

## Table of Contents  
- [Tools Used](#tools-used)  
- [Circuit Description](#circuit-description)  
- [Design Specifications](#design-specifications)  
- [Simulation Results](#simulation-results)  
- [Layout and Analysis](#layout-and-analysis)  
- [Future Scope](#future-scope)  
- [Contributor](#contributor)  
- [Acknowledgments](#acknowledgments)  

---

## Tools Used  
- **eSim** – Open-source EDA tool developed by *FOSSEE, IIT Bombay*, integrating KiCad, Ngspice, and GHDL.  
- **Ngspice** – Open-source SPICE simulator for analog and mixed-signal circuit analysis.  
- **Magic** *(optional, for layout)* – Open-source VLSI layout editor for Sky130 PDK and other technologies.  

---

## Circuit Description  
The amplifier consists of **two stages**:  

1. **Differential Amplifier Stage** – Transistors M1–M4 form a differential pair with active loads, converting differential input into single-ended output with high gain.  
2. **Gain Stage** – A PMOS common-source amplifier (M6) with active NMOS load increases overall voltage gain and swing.  

A **600 fF compensation capacitor** ensures stability, and a **2 pF load capacitor** models the output load.  

 

---

## Design Specifications  

| Parameter | Value |
|------------|--------|
| Supply Voltage | 1.8 V |
| DC Gain | 90 – 100 dB |
| Phase Margin | ≈ 60° |
| Load Capacitance | 2 pF |
| Compensation Capacitance | 600 fF |

---

## Simulation Results  
Simulations were performed in **Ngspice** using `.cir` files generated from eSim.  
- **DC Gain and Frequency Response** confirm high gain and stability.  
- **Phase Margin ≈ 60°** indicates good compensation.  

---

## Layout and Analysis  
If layout is designed using **Magic** and **Sky130 PDK**, post-layout simulation can be done to compare results with pre-layout analysis.  

---

## Future Scope  
- Implement using **Sky130 PDK** for fabrication-level verification.  
- Optimize transistor sizing for higher bandwidth and lower power.  
- Extend to **fully differential** or **folded-cascode** architectures.  

---

## Contributor  
**Mihir Kumar Behera**  
B.Tech, Dept. of Electronics and Communication Engineering  
National Institute of Technology, Rourkela  
📧 *mihir79kumar@gmail.com*  

---

## Acknowledgments  
Special thanks to the **FOSSEE eSim Team, IIT Bombay**, for providing open-source EDA tools and guidance under the **FOSSEE Circuit Simulation Project** initiative.  
