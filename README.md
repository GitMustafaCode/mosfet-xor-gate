# MOSFET-Based XOR Gate

This project demonstrates the design, construction, and testing of a 2-input XOR logic gate using discrete MOSFET transistors. The XOR gate was built using transistor-level design methodology.

For detailed calculations on design decisions please refer to this document: [Project Document](https://github.com/GitMustafaCode/mosfet-xor-gate/blob/main/project_doc.pdf)

---

## 🔧 Objective

Design, build, and test a functional XOR logic gate entirely using MOSFET transistors on a breadboard. The circuit was analyzed for logical functionality, voltage levels, and timing performance.

---

## ⚙️ Circuit Schematic

The XOR gate was designed using 12 transistors from two **MC14007UB** ICs, following standard CMOS design practices. The schematic includes the PMOS and NMOS transistors arranged to realize the XOR logic truth table.

![image](https://github.com/GitMustafaCode/mosfet-xor-gate/blob/main/Schematic.png)

The transistors are labeled clearly, with pull-up and pull-down networks formed to handle each logic input combination correctly.

---

## ✅ Functional Testing

The physical circuit was constructed on a breadboard and tested using an **Analog Discovery 2** (AD2) for input pattern generation and output analysis.

![image](https://github.com/user-attachments/assets/90c8b9e4-c7d3-4b31-a623-07d51ea7092d)

### Input-Output Patterns

Logic analyzer results confirmed the XOR functionality:

- Y = 0 when A = B (both 0 or both 1)
- Y = 1 when A ≠ B

![image](https://github.com/user-attachments/assets/e7c82c64-5c78-4a40-a170-49f4394d2522)

---

## 📉 Static Voltage Level Testing

To evaluate output voltage levels:

- One input (A) was fixed at 5V (logic HIGH)
- The other input (B) was toggled with a square wave (0-5V)
- The output (Y) was measured on an oscilloscope

### Results

- **VH (High):** ~5.05 V
- **VL (Low):** ~0 V

![image](https://github.com/user-attachments/assets/8fda82f2-ffbe-431b-9fe7-dc51979d308e)

---

## 📁 Files Included

- `XOR.asc`: XOR circuit schematic
- `project_doc.pdf`: Detailed Explanation

---
