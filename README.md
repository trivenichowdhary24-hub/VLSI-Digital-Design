# Fundamental Digital Logic Gates Library

This repository contains my very first hardware description project as part of my 3rd-year VLSI specialization and GATE preparation journey. It features a unified, synthesizable Verilog implementation of all seven foundational logic gates alongside a verification testbench.
##implemented circuits
The  design file (`basic_gates.v`) models the following 2-input logic operations using continuous behavioral assignments:
*   **AND** (`&`)
*   **OR** (`|`)
*   **NOT** (`~` - *Inverts Input A*)
*   **NAND** (`~&`)
*   **NOR** (`~|`)
*   **XOR** (`^`)
*   **XNOR** (`~^`)

## Simulation & Verification
The testbench script (`basic_gates_tb.v`) systematically cycles through the complete 2-bit binary truth table sequence (`00`, `01`, `10`, `11`) at a `1ns/1ps` timescale to verify functional accuracy. Output logic levels are monitored dynamically using the automated `$monitor` task.

### Expected Console Output Log
```text
Time=0  | A=0 B=0 | AND=0 OR=0 NOT_A=1 NAND=1 NOR=1 XOR=0 XNOR=1
Time=10 | A=0 B=1 | AND=0 OR=1 NOT_A=1 NAND=1 NOR=0 XOR=1 XNOR=0
Time=20 | A=1 B=0 | AND=0 OR=1 NOT_A=0 NAND=1 NOR=0 XOR=1 XNOR=0
Time=30 | A=1 B=1 | AND=1 OR=1 NOT_A=0 NAND=0 NOR=0 XOR=0 XNOR=1
```
- [x] Basic Logic Gates & Unified Testbenches
- [ ] Combinational Circuits (Half/Full Adder, Multiplexers)
- [ ] Sequential Circuits (Flip-Flops, Shift Registers, Counters)
- [ ] Industry Tool Simulation (Cadence Virtuoso/Xcelium Integration)
-
