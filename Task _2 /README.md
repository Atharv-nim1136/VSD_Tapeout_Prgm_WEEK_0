````markdown
# 🚀 **VLSI System Design (VSD) Program**

![Week 0: VLSI System Design (VSD) Program Foundation & Tool Setup](https://img.shields.io/badge/Week_0-FOUNDATION_&_TOOL_SETUP-blue)
![Status: Complete](https://img.shields.io/badge/STATUS-COMPLETE-green)

Welcome to my **VLSI System Design (VSD) Program** repository! This week focused on setting up the development environment and installing the essential open-source tools that will be used throughout the program. The goal was to create a reliable and efficient workspace for synthesis, simulation, and design tasks.

***

### ⚙️ **System and Virtual Machine Configuration**

To ensure optimal performance, I configured a Virtual Machine (VM) named `Atharv_nim_1136` with the following specifications:

| Specification 💻 | Details 📋 |
| :--- | :--- |
| **Operating System** 🐧 | Ubuntu 20.04+ |
| **RAM** 💾 | 6GB |
| **Storage** 💿 | 50GB HDD |
| **vCPUs** ⚡ | 4 |

> **💡 Pro Tip:** This setup guarantees sufficient resources for handling toolchain demands and running simulations smoothly.

***

### 🛠️ **Tool Installation & Verification**

The following tools were installed for RTL synthesis, simulation, circuit analysis, and layout design. Below are the installation steps and verification commands.

| **🧠 Yosys** | **📟 Iverilog** | **📊 GTKWave** | **⚡ Ngspice** | **🎨 Magic VLSI** |
| :---: | :---: | :---: | :---: | :---: |

#### 🧠 **1. Yosys – RTL Synthesis Tool**

**Purpose:** Converts RTL code into gate-level representations. Yosys is a framework for Verilog RTL synthesis, providing synthesis algorithms and optimization passes for digital circuits.

**✅ Yosys Installation**

```bash
# Day 0 - Tools Installation
## Yosys

$git clone [https://github.com/YosysHQ/yosys.git$](https://github.com/YosysHQ/yosys.git$) cd yosys 
$ sudo apt install make # (If make is not installed please install it) 
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make 
$ sudo make install
````

-----

#### 📟 **2. Iverilog – Verilog Simulator**

**Purpose:** Compiles and simulates Verilog designs for functional verification. Icarus Verilog is a Verilog simulation and synthesis tool that supports the IEEE-1364 Verilog HDL standard.

**✅ Iverilog Installation**

```bash
$ sudo apt-get install iverilog
```

-----

#### 📊 **3. GTKWave – Waveform Viewer**

**Purpose:** Analyzes and visualizes simulation waveforms for debugging. GTKWave is a fully featured GTK+ based wave viewer for Unix, Win32, and Mac OSX.

**✅ GTKWave Installation**

```bash
$ sudo apt update
$ sudo apt install gtkwave
```

-----

#### ⚡ **4. Ngspice – Circuit Simulator**

**Purpose:** Performs analog and mixed-signal circuit simulation. Ngspice is a mixed-level/mixed-signal circuit simulator based on Spice3f5, Cider1b1 and Xspice.

**✅ Ngspice Installation**

```bash
$ sudo apt update
$ sudo apt install ngspice
```

-----

#### 🎨 **5. Magic VLSI – Layout Tool**

**Purpose:** Creates, edits, and analyzes VLSI layouts with DRC capabilities. Magic VLSI is an open-source VLSI layout tool widely used for IC design, DRC, and visualization.

**✅ Magic VLSI Installation**

```bash
# Install required dependencies
sudo apt-get install m4
sudo apt-get install tcsh
sudo apt-get install csh
sudo apt-get install libx11-dev
sudo apt-get install tcl-dev tk-dev
sudo apt-get install libcairo2-dev
sudo apt-get install mesa-common-dev libglu1-mesa-dev
sudo apt-get install libncurses-dev

# Clone Magic repository
git clone [https://github.com/RTimothyEdwards/magic](https://github.com/RTimothyEdwards/magic)
cd magic

# Configure build
./configure

# Build Magic
make

# Install system-wide
sudo make install
```

-----

### 🎉 **Installation Summary**

| Tool | Status | Primary Use |
| :--- | :---: | :--- |
| 🧠 **Yosys** | ✅ Complete | RTL Synthesis |
| 📟 **Iverilog** | ✅ Complete | Verilog Simulation |
| 📊 **GTKWave** | ✅ Complete | Waveform Analysis |
| ⚡ **Ngspice** | ✅ Complete | Circuit Simulation |
| 🎨 **Magic VLSI** | ✅ Complete | Layout Design |

-----

### 🚀 **Environment Ready for VLSI Design Journey\!**

| 📂 Repository | **RTL2GDS\_Alchemy** |
| :--- | :--- |
| 👨‍💻 Author | **Atharv\_nim\_1136** |
| 📚 Program | **VLSI System Design (VSD)** |

```
```
