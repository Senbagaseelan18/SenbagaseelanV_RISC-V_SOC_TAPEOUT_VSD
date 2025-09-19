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

## 🛠️ Tool 1: Yosys  

**Yosys** is an open-source framework for RTL synthesis, primarily used for Verilog designs.  
It converts high-level Verilog RTL into gate-level netlists that can be used for simulation and layout.  

### 🔽 Installation Steps  

```bash
# Update packages
$ sudo apt-get update  

# Clone Yosys repository
$ git clone https://github.com/YosysHQ/yosys.git  
$ cd yosys  

# Install required dependencies
$ sudo apt install make               # If make is not installed  
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev  

# Configure with GCC
$ make config-gcc  

# Initialize submodules
$ git submodule update --init --recursive  

# Build Yosys
$ make  

# Install Yosys
$ sudo make install  

### 📌 Notes & Tips  
- 🟢 More RAM = faster simulations and fewer slowdowns.  
- 🟢 SSD storage instead of HDD can **significantly reduce tool load times**.  
- 🟢 Keep your system updated for compatibility with open-source EDA tools.  

---
