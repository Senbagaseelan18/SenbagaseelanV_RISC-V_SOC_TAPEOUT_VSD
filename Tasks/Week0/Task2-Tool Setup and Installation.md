# ⚙️ Tools Installation – VSD Program Setup

<div align="center">

![Tools](https://img.shields.io/badge/Tools-Installation-blue?style=for-the-badge&logo=tools)
![Setup](https://img.shields.io/badge/Setup-Ready-success?style=for-the-badge)
![VLSI](https://img.shields.io/badge/VLSI-System%20Design-orange?style=for-the-badge&logo=chip)

</div>

Welcome to the **Tools Installation Guide** for the **VLSI System Design (VSD) Program**.  
This section ensures that all the required tools and dependencies are properly installed to create a smooth workflow for RTL design, simulation, and layout.  

---

## 🖥️ **System Requirements**

To guarantee stable performance during synthesis, simulation, and layout design, ensure your system meets the following specifications:

<div align="center">

| **Specification** 💻    | **Requirement** 📋      |
|--------------------------|-------------------------|
| **Operating System** 🐧  | Ubuntu 20.04 or higher |
| **RAM** 💾               | 6 GB                   |
| **Storage** 💿           | 50 GB HDD              |
| **vCPUs** ⚡             | 4                      |

</div>

> 💡 **Pro Tip:** Allocating slightly higher resources (like 8 GB RAM) can further improve simulation speed and tool performance.

---

## 📂 **Installation Instructions**

Below are the installation steps for all required tools:  

---

### 1️⃣ **Yosys** — RTL Synthesis
```bash
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
$ git submodule update --init --recursive
$ make 
$ sudo make install
