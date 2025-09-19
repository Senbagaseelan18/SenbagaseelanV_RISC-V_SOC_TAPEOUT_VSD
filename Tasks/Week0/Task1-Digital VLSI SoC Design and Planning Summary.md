# Task 1 — Digital VLSI SoC Design and Planning

## 📌 Introduction

This document summarizes the core concepts of **Digital VLSI SoC design and planning**, covering the flow from chip modeling to SoC integration and verification. It is intended as the Week0 submission for the course.

---

## 🔹 Chip Modeling (O1)

* Start with **chip specifications** (often a C model).
* Specifications define expected functionality and interfaces.
* Validate the spec with a **C testbench** to confirm behavior before RTL.

---

## 🔹 RTL Architecture (O2)

* Implement the hardware in **RTL (Verilog)** — the soft copy of the design.
* Break the design into major blocks: **Processor** and **Peripherals / IPs**.
* Verify RTL against the C model/spec to ensure functional equivalence.

---

## 🔹 Synthesis & Netlist

* Synthesize RTL to produce a **Gate-Level Netlist (GLN)**.
* Outputs include synthesized macros and functional analog IP models.

---

## 🔹 SoC Integration (O3)

* Integrate processor, peripherals, and IPs into the SoC top-level.
* Perform floorplanning, placement, CTS (clock tree synthesis), and routing.
* Integrate hardened macros (HMs) and analog IP libraries as needed.
* The physical layout output is a **GDSII** file for fabrication.

---

## 🔹 Physical Verification

* Run **DRC (Design Rule Check)** and **LVS (Layout vs Schematic)** to ensure manufacturability and schematic/layout consistency.

---

## 🔹 Final SoC (O4)

* Target operating frequency range: **\~10 MHz – 130 MHz** (as an example).
* The same SoC architecture can be adapted to different end-products (e.g., wearable, microcontroller boards, display electronics, HVAC controllers) by changing peripherals/IP sets.

---

## ✅ Key Takeaways

* Typical flow: **Chip Spec (C) → RTL (Verilog) → Synthesis → SoC Integration → Physical Verification → Final GDSII**.
* Verification at every stage is crucial to ensure functional correctness and manufacturability.
* Modular design (processor + peripherals + IPs) enables reuse across multiple applications.

---

## 📁 Suggested repository placement

Place this file at: `Tasks/Week0/task1_digital_vlsi_soc_design_and_planning.md` and include any relevant screenshots under `Tasks/Week0/media/`.

---

*Prepared by: Senbagaseelan V — RISC-V SoC Tapeout — VSD*
