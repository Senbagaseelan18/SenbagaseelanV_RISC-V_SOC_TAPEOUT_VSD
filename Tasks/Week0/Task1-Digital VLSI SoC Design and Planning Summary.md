# 📝 Task 1 — Summary of Digital VLSI SoC Design and Planning

## 📌 Introduction
This document provides a **summary of Digital VLSI SoC Design and Planning**, highlighting the end-to-end flow from **chip modeling** to **final SoC integration**.  
It captures the key design stages, verification steps, and the importance of modular SoC architecture.

---

## 🔹 O1 — Chip Modeling
- Starts with **chip specifications** (C model).  
- Functionality validated using a **C testbench**.  
- Ensures design intent and expected behavior are correct **before RTL implementation**.  

---

## 🔹 O2 — RTL Architecture
- Hardware described in **RTL (Verilog)** — the *soft copy of hardware*.  
- Design partitioned into major blocks:  
  - 🖥️ **Processor**  
  - 🔌 **Peripherals / IPs**  
- RTL verified against the spec to ensure correctness.  

---

## 🔹 Synthesis & Netlist Generation
- RTL synthesized into a **Gate-Level Netlist (GLN)**.  
- Outputs include:  
  - ✅ Gate-Level Netlist  
  - ✅ Synthesized macros  
  - ✅ Analog IPs (functional models)  

---

## 🔹 O3 — SoC Integration
- Integration of processor, peripherals, and IPs into a **System-on-Chip**.  
- Involves:  
  - 📐 Floorplanning  
  - 🕒 Clock Tree Synthesis (CTS)  
  - 🛠️ Placement & Routing  
- Hardened macros and analog IP libraries are added.  
- Final output: **GDSII file** for chip fabrication.  

---

## 🔹 Physical Verification
- ✅ **DRC (Design Rule Check)** → Ensures design follows manufacturing rules.  
- ✅ **LVS (Layout vs Schematic)** → Confirms physical layout matches schematic.  

---

## 🔹 O4 — Final SoC
- Operates in the **10 MHz – 130 MHz** range.  
- Adaptable to multiple applications by changing peripherals/IPs:  
  - ⌚ iWatch  
  - 🔌 Arduino boards  
  - 📺 TV panels  
  - ❄️ AC systems  

---

## ✅ Key Takeaways
- **Complete Flow:** Specs → RTL → Synthesis → SoC Integration → Verification → Final Chip.  
- **Verification at each stage** ensures functionality and manufacturability.  
- **Reusable modular design** allows targeting different real-world applications.  

---

📂 **File Location Recommendation:**  
`Tasks/Week0/task1_summary_digital_vlsi_soc_design_and_planning.md`

✍️ *Prepared by: Senbagaseelan V — RISC-V SoC Tapeout (VSD)*  
