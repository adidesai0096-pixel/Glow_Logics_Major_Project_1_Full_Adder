# Design and Performance Analysis of a CMOS 1-Bit Full Adder Using LTspice

## Project Overview

This project focuses on the transistor-level design, simulation, and functional verification of a CMOS 1-bit Full Adder using LTspice.

The Full Adder is a fundamental combinational logic circuit used in arithmetic and digital systems. It performs binary addition of three input bits and generates two outputs: Sum and Carry.

This project was completed as **Major Project 1** under the **Glow Logics VLSI Internship Program**.

## Internship Details

- **Organization:** Glow Logics
- **Program:** VLSI Internship
- **Project Category:** Major Project 1
- **Project Title:** CMOS 1-Bit Full Adder
- **Simulation Tool:** LTspice 26.1.1
- **Design Technology:** CMOS Transistor-Level Design

## Objectives

- Design a 1-bit Full Adder using CMOS logic.
- Implement the circuit using transistor-level NAND gates.
- Understand PMOS and NMOS transistor operation.
- Simulate the circuit using LTspice.
- Verify the Sum and Carry outputs using all eight input combinations.
- Study important performance parameters such as power consumption and propagation delay.

## Circuit Architecture

The Full Adder is implemented using **9 CMOS NAND gates**.

Each 2-input CMOS NAND gate consists of:
- 2 PMOS transistors connected in parallel.
- 2 NMOS transistors connected in series.

Therefore, the complete design contains:

- Number of NAND gates: 9
- PMOS transistors: 18
- NMOS transistors: 18
- **Total MOSFETs: 36**

## Boolean Expressions

**Sum:**

`SUM = A XOR B XOR Cin`

**Carry:**

`COUT = AB + ACin + BCin`

## Truth Table

| A | B | Cin | SUM | COUT |
|---|---|---|---|---|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 |
| 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |

## Simulation Details

The circuit was simulated in LTspice using a 1.8 V supply voltage.

- Supply voltage: 1.8 V
- Transient analysis: 40 ms
- Input signals: A, B and Cin
- Outputs observed: SUM and COUT

The transient simulation verified the expected Full Adder truth table for all eight input combinations.

## Performance Analysis

An average supply-power measurement was performed using LTspice.

Measured average power:

`Pavg = 7.8724 × 10⁻¹¹ W`

This corresponds to approximately 78.72 pW for the specified simulation measurement expression and interval. The supply node and current sign convention should be confirmed before treating this as a final power-performance result.

Propagation delay measurements were explored, but the available measurements were not validated. Therefore, no final propagation-delay value is claimed.

## Tools and Technologies

- LTspice 26.1.1
- CMOS Logic Design
- PMOS and NMOS Transistors
- Transient Analysis
- Digital Circuit Simulation

## Project Files

- `CMOS_Full_Adder_Transistor_Level.asc` – LTspice circuit schematic
- `Glow_Logics_VLSI_Internship_Major_Project_1_Full_Adder_Report.pdf` – Detailed project report
- Simulation screenshots – Circuit and output waveforms

## Learning Outcomes

Through this project, I gained practical experience in:

- CMOS transistor-level circuit design.
- Implementing digital logic using NAND gates.
- Understanding PMOS and NMOS configurations.
- Creating and debugging LTspice schematics.
- Performing transient simulations.
- Verifying digital outputs using truth tables.
- Exploring power measurement in CMOS circuits.

## Future Scope

- Compare different CMOS Full Adder architectures.
- Investigate propagation delay under controlled input transitions.
- Compare power consumption across different logic styles.
- Explore layout design and physical implementation.

## Acknowledgement

I would like to thank **Glow Logics** for providing the opportunity to work on this VLSI internship project and gain practical experience in CMOS digital circuit design and simulation.

---

**Project developed as part of the Glow Logics VLSI Internship Program.**

**Author:** Aditya Ramakant Desai
