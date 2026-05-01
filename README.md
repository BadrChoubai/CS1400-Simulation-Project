# CS1400: 7-Segment Display Decoder Final Project

A combinational logic circuit that decodes a 3-bit input into four distinct digits, displayed on a 7-segment output, designed and simulated in Logisim-Evolution.

**Deliverables**:

- [Truth Table](./truth-table.md)
- [K-Maps](./k-maps.md)
- [Logisim Circuits](./circuit.md)

## Overview

This project implements a custom decoder for four specific digits derived from a student ID. Given a 3-bit binary input (X, Y, Z), the circuit drives the correct segment signals (a–g) to display the corresponding digit on a 7-segment display.

The design follows the full digital logic pipeline:

1. **Truth table**: mapping every input combination to its required segment outputs
2. **Karnaugh maps**: minimizing Boolean expressions for each of the 7 output signals
3. **Combinational circuit**: implementing the simplified logic in Logisim-Evolution

This project demonstrates the foundational hardware design process that underlies every digital system from calculators to CPUs.

## Digits Decoded

|  X  |  Y  |  Z  | Digit Displayed |
| :-: | :-: | :-: | :-------------: |
|  0  |  0  |  0  |        n        |
|  0  |  0  |  1  |        6        |
|  0  |  1  |  0  |        9        |
|  0  |  1  |  1  |        3        |
|  1  |  0  |  0  |        -        |
|  1  |  0  |  1  |        -        |
|  1  |  1  |  0  |        -        |
|  1  |  1  |  1  |        -        |

## Design Process

> ### Truth Table
>
> The truth table maps each 3-bit input to the ON/OFF state of all 7 segments. The upper four rows (X = 0) are fully specified; the lower four rows (X = 1) are don't-care conditions used to simplify the K-map expressions. [Read More](./truth-table.md)
>
> ### Karnaugh Maps
>
> One K-map was constructed per output segment (a through g). Don't-care conditions (X = 1) were exploited where possible to expand groupings and reduce gate count. [Read More](./k-maps.md)
>
> ### Combinational Circuit
>
> The simplified Boolean expressions were implemented in **Logisim-Evolution** using AND, OR, and NOT gates. The circuit takes three input pins (X, Y, Z), routes them through the gate logic derived from the K-maps, and drives a 7-segment display component directly. [Read More](./circuit.md)

## Course Context

Built as a final project for a **Computer Organzation** course. The assignment required applying truth tables, K-map minimization, and combinational circuit design to a real display decoding problem.

## Skills Demonstrated

- Boolean algebra and logic minimization (Karnaugh maps)
- Combinational circuit design with don't-care conditions
- Digital simulation with Logisim-Evolution
- Hardware-software boundary thinking (how displays work at the gate level)
