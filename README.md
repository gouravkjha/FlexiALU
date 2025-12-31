# FlexiALU

FlexiALU is a parameterizable signed ALU written in Verilog. It supports arithmetic (ADD/SUB), logic (AND/OR/XOR), shift, and rotate operations with zero, sign, and overflow flags. The design is suitable for FPGA implementation and has been verified using Vivado and EDA Playground.

---

## Features
- Parameterizable data width (default: 8-bit)
- Signed arithmetic operations:
  - Addition
  - Subtraction
- Logic operations:
  - AND
  - OR
  - XOR
- Shift operations:
  - Arithmetic right shift
  - Logical left shift
- Rotate operations:
  - Rotate left
  - Rotate right
- Status flags:
  - Zero flag
  - Sign flag
  - Overflow flag

---

## Operation Selection

| Operation | Select Code |
|---------|-------------|
| ADD | `0000` |
| SUB | `0001` |
| AND | `0010` |
| OR  | `0011` |
| XOR | `0100` |
| Shift Right (A) | `0101` |
| Shift Left (A)  | `0110` |
| Shift Left (B)  | `0111` |
| Shift Right (B) | `1000` |
| Rotate Right (A)| `1001` |
| Rotate Left (B) | `1010` |

---

## Simulation

### Online Simulation
You can simulate this ALU online using **EDA Playground**:  
 https://www.edaplayground.com/x/cXqH

### Local Simulation
The design has been tested using **Xilinx Vivado Simulator**.

---

## Project Structure

| Folder | File | Description |
|------|------|------------|
| src | alu_top.v | Top-level ALU |
| src | arithmetic_unit.v | Arithmetic operations |
| src | logic_unit.v | Logical operations |
| src | shift_rotate_unit.v | Shift & rotate |
| tb | alu_tb.v | Testbench |
| mem | test_vectors.mem | Test vectors |

---


## Download

You can download the complete FlexiALU Verilog code folder here:  

[Download FlexiALU.zip](https://github.com/user-attachments/files/24395394/FlexiALU.zip)

---



## Tools & Technologies:
- Verilog HDL (IEEE 1364)
- Xilinx Vivado (simulation)
- EDA Playground


---

## License
This project is licensed under the MIT License.
