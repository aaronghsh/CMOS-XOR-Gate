# CMOS XOR Gate using MOSFETs 🧠

This project demonstrates the implementation of a functional XOR gate using **MOSFETs** on **CD4007B CMOS ICs**. The project includes full circuit simulation, physical hardware construction, logic verification, and signal timing analysis.

---

## Project Objective

Design and test a **CMOS XOR logic gate** using discrete MOSFETs, ensuring:
- Functional logic operation (truth table verification).
- Clean HIGH/LOW transitions with minimal noise.
- Acceptable **rise/fall times** and **propagation delay**.
- Real-world validation using **Analog Discovery 3 (AD3)**.

---

## Technologies & Tools Used

- **CD4007B CMOS ICs**: Provide NMOS and PMOS pairs.
- **Analog Discovery 3 (AD3)**: Used for waveform generation, logic analyzer, and scope.
- **Breadboard & Passive Components**: Used for physical implementation.
- **100nF Capacitor**: Used as a capacitive load for dynamic testing.

---

## Features

- **CMOS-Based XOR Logic**:
  - Built using 6 NMOS and 6 PMOS transistors from two CD4007B ICs.
  - Mimics ideal transistor sizing with an approximate 5:2 PMOS:NMOS ratio.
- **Truth Table Verification**:
  - Inputs (A, B) tested through all combinations: 00, 01, 10, 11.
  - Output matched standard XOR behavior.
- **Static Testing**:
  - Input A held constant while input B varied as a square wave.
  - Voltage swing measured from ≈5V to ≈30mV, confirming sharp logic levels.
- **Dynamic Timing Analysis**:
  - Rise Time: 485 μs  
  - Fall Time: 316 μs  
  - Propagation Delay (average): 582.5 μs

---

## Circuit Overview

- **ICs Used**: CD4007B (x2)
- **Design Constraints**:
  - Manual transistor sizing not possible with IC.
  - Logic powered via AD3 module (5V).
  - Gate verified via Logic Analyzer (DIO channels).
- **Capacitive Load**:
  - A 100nF capacitor was added to simulate dynamic behavior during output transitions.

---

## Project Files

- `Project 4.asc`: CMOS logic schematic for XOR gate.
- `Project 4 Documentation.pdf`: Full report with circuit description, testing, and analysis.
