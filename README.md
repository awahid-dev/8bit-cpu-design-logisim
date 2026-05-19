# Custom Hybrid Multi-Cycle CPU in Logisim

## Overview
This project is a fully custom-designed **Hybrid Multi-Cycle CPU** built entirely in **Logisim Evolution** from scratch.

The architecture combines concepts from both **Accumulator-Based** and **General Purpose Register (GPR)** CPUs, creating a unique hybrid execution model.  
The CPU executes instructions over multiple clock cycles using a custom hardwired control unit and modular datapath design.

The project focuses on understanding how real processors work internally — from instruction fetch and decode to ALU execution, flag generation, control signal routing, and program flow control.

---

## CPU Architecture

### Core Components
- Arithmetic Logic Unit (ALU)
- Accumulator Register
- General Purpose Register System
- Instruction Register (IR)
- Program Counter (PC)
- Program ROM
- Flag Register
- Instruction Decoder
- Jump Decoder
- Multi-cycle Hardwired Control Unit

---

## Key Features

### Hybrid CPU Design
Unlike a pure accumulator CPU or pure register-based CPU, this processor combines both approaches:
- Fast accumulator-based ALU operations
- Register-assisted data handling
- Shared datapath architecture

---

### Multi-Cycle Execution
Each instruction is divided into multiple stages:
1. Instruction Fetch
2. Instruction Decode
3. Operand Routing
4. ALU Execution
5. Register Write Back

This reduces hardware complexity while improving control flexibility.

---

### Custom Hardwired Control Unit
The control unit generates timing-based control signals using:
- Instruction decoding
- Timing states
- Control gating logic
- Conditional execution paths

---

### ALU and Flag System
The ALU supports multiple arithmetic and logical operations with integrated:
- Zero Flag
- Carry Flag
- Sign/Negative Flag
- Overflow handling support

Flags are stored inside a dedicated flag register for conditional operations.

---

### Program Flow Control
The CPU currently supports:
- Sequential execution
- Jump instructions
- Conditional branching logic foundation
- Program Counter based instruction addressing

---

## Current Progress

### Completed
- ALU design and integration
- Accumulator datapath
- Register routing system
- Program Counter implementation
- Instruction Register implementation
- Instruction decoding system
- Jump decoding logic
- Program ROM integration
- Multi-cycle timing system
- Hardwired control signal generation
- Flag generation and storage
- Display output integration

---

## Instruction Set (Current)

| Opcode Type | Description |
|---|---|
| LOAD | Load data into accumulator/register |
| ADD | Arithmetic addition |
| SUB | Arithmetic subtraction |
| AND | Logical AND |
| OR | Logical OR |
| JMP | Unconditional jump |
| Conditional Jump | Branch using flags |
| DISPLAY | Output/display operation |

---

## Design Goals
- Learn processor architecture deeply
- Build a CPU completely from logic level
- Understand datapath and control interaction
- Explore instruction cycle execution
- Prepare foundation for future advanced CPU features

---

## Future Plans

### Memory Expansion
- RAM integration
- MAR (Memory Address Register)
- Read/Write instruction support

### ISA Improvements
- Expanded instruction format
- More ALU operations
- Better addressing modes

### Advanced Features
- Stack support
- Subroutine calls
- Interrupt handling
- Pipelining experiments
- Basic cache concepts

---

## Built With
- **Logisim Evolution**
- Digital Logic Design
- Custom CPU Architecture Concepts

---


## Author
**Wahid**  
Creator of a custom hybrid CPU architecture in Logisim Evolution.
