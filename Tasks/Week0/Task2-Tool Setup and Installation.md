# ⚙️ VSD Program – Tools Installation Guide  

<div align="center">

🌐 **One place for all your VLSI tool setup needs**  

✨ Smooth Installation · ⚡ Optimized Performance · 🛠️ Ready for Design  

</div>  

---

## 🖥️ **Before You Begin – System Checklist**  

Make sure your system is ready for synthesis, simulation, and layout by meeting the **minimum hardware/software requirements** below:  

<div align="center">

| 🔧 **Component** | ✅ **Recommended Setup** |
|------------------|--------------------------|
| 🐧 **OS**        | Ubuntu 20.04 LTS or newer |
| 💾 **Memory**    | 6 GB (8 GB+ preferred 🚀) |
| 💿 **Disk**      | 50 GB free storage |
| ⚡ **CPU Cores** | 4 vCPUs (multi-core boosts speed) |

</div>  

---

# 📂 Installation Instructions  

All detailed steps for installing **Yosys**, **Iverilog**, **GTKWave**, **Ngspice**, and **Magic VLSI** can be found in the upcoming sections.  

---

### 🧠 **1. Yosys – RTL Synthesis Tool**

<details>
<summary><b>Purpose:</b> Converts RTL code into gate-level representations.</summary>

</details>
Yosys is an open-source framework for Verilog RTL synthesis, offering algorithms and optimization passes to transform RTL into gate-level netlists for further simulation and physical design.

---

## ✅ **Yosys Installation**

```bash
# Day 0 - Tools Installation
## Yosys

# Clone Yosys repository
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys 

# Install make (if not installed)
$ sudo apt install make 

# Install dependencies
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev

# Configure build with GCC
$ make config-gcc

# Initialize Git submodules (required for abc)
$ git submodule update --init --recursive

# Build Yosys
$ make 

# Install Yosys
$ sudo make install
```

## 📷 **Installation Verification**

```bash
# Run Yosys after installation
$ yosys
```

<p align="center">
  <img src="https://github.com/Senbagaseelan18/SenbagaseelanV_RISC-V_SOC_TAPEOUT_VSD/blob/main/Tasks/Week0/images/yosys.png" 
       alt="Yosys Installed" width="600"/>
</p>

<div align="center">

✅ **Yosys Successfully Installed**

</div>

### 🧠 **2. Iverilog – Verilog Simulator**

<details>
<summary><b>Purpose:</b> Compiles and simulates Verilog designs for functional verification.</summary>

</details>
Iverilog is an open-source Verilog simulation and compilation tool. It allows you to compile Verilog code into executable simulations and run functional verification of your designs before synthesis.

---

## ✅ **Iverilog Installation**

```bash
# Install Iverilog
$ sudo apt-get install iverilog
```

## 📷 **Installation Verification**

```bash
# Run Iverilog after installation
$ iverilog 
```

<p align="center">
  <img src="images/iverilog.png" 
       alt="Iverilog Installed" width="600"/>
</p>

<div align="center">
  ✅ <b>Iverilog Successfully Installed</b>
</div>

### 🧠 **3. GTKWave – Waveform Viewer**

<details>
<summary><b>Purpose:</b> Analyzes and visualizes simulation waveforms for debugging.</summary>

</details>
GTKWave is an open-source waveform viewer used to analyze and visualize simulation outputs from Verilog and VHDL. It helps in debugging designs by displaying signal waveforms clearly.

---

## ✅ **GTKWave Installation**

```bash
# Update packages
$ sudo apt update

# Install GTKWave
$ sudo apt install gtkwave
```

## 📷 **Installation Verification**

```bash
# Run GTKWave after installation
$ gtkwave 
```
<p align="center">
  <img src="images/gtkwave.png" 
       alt="GTKWave Installed" width="600"/>
</p>

<div align="center">
  ✅ <b>GTKWave Successfully Installed</b>
</div>



