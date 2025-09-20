# **🚀 VSD Program: Foundation & Tool Setup**

Welcome to my **VLSI System Design (VSD) Program** repository\! This week focused on setting up the development environment and installing the essential open-source tools that will be used throughout the program. The goal was to create a reliable and efficient workspace for synthesis, simulation, and design tasks.

### **💻 System and Virtual Machine Configuration**

To ensure optimal performance, I configured a **Virtual Machine (VM)** named **`Atharv_nim_1136`** with the following specifications:

| Specification 💻 | Details 📋 |
| :--- | :--- |
| **Operating System** 🐧 | Ubuntu 20.04+ |
| **RAM** 💾 | 6GB |
| **Storage** 💿 | 50GB HDD |
| **vCPUs** ⚡ | 4 |

> **💡 Pro Tip:** This setup guarantees sufficient resources for handling toolchain demands and running simulations smoothly.

-----

### **🛠️ Tool Installation & Verification**

The following tools were installed for RTL synthesis, simulation, circuit analysis, and layout design.

| **🧠 Yosys** | **📟 Iverilog** | **📊 GTKWave** | **⚡ Ngspice** | **🎨 Magic VLSI** |
| :---: | :---: | :---: | :---: | :---: |

#### 🧠 **1. Yosys – RTL Synthesis Tool**

**Purpose:** Converts RTL code into gate-level representations.

**Installation Commands:**

```bash
sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make
sudo apt-get install build-essential clang bison flex libreadline-dev gawk tcl-dev libffi-dev git graphviz xdot pkg-config python3 libboost-system-dev libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install
```

#### 📟 **2. Iverilog – Verilog Simulator**

**Purpose:** Compiles and simulates Verilog designs for functional verification.

**Installation Commands:**

```bash
sudo apt-get update
sudo apt-get install iverilog
```

#### 📊 **3. GTKWave – Waveform Viewer**

**Purpose:** Analyzes and visualizes simulation waveforms for debugging.

**Installation Commands:**

```bash
sudo apt-get update
sudo apt install gtkwave
```

#### ⚡ **4. Ngspice – Circuit Simulator**

**Purpose:** Performs analog and mixed-signal circuit simulation.

**Installation Commands:**

```bash
# After downloading the tarball from https://sourceforge.net/projects/ngspice/files/
tar -zxvf ngspice-37.tar.gz
cd ngspice-37
mkdir release
cd release
../configure --with-x --with-readline=yes --disable-debug
make
sudo make install
```

#### 🎨 **5. Magic VLSI – Layout Tool**

**Purpose:** Creates, edits, and analyzes VLSI layouts with DRC capabilities.

**Installation Commands:**

```bash
sudo apt-get install m4 tcsh csh libx11-dev tcl-dev tk-dev libcairo2-dev mesa-common-dev libglu1-mesa-dev libncurses-dev
git clone https://github.com/RTimothyEdwards/magic
cd magic
./configure
make
sudo make install
```

#### **6. OpenLane**

**Purpose:** An automated RTL-to-GDSII flow that takes a design from RTL to a final chip layout.

**Installation Commands:**

```bash
sudo apt-get update
sudo apt-get upgrade
sudo apt install -y build-essential python3 python3-venv python3-pip make git
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io
sudo docker run hello-world
sudo groupadd docker
sudo usermod -aG docker $USER
sudo reboot
# After reboot:
docker run hello-world

# Install PDKs and Tools
cd $HOME
git clone https://github.com/The-OpenROAD-Project/OpenLane
cd OpenLane
make
make test
```

-----

### **🎉 Installation Summary**

This table provides a quick overview of the installed tools and their primary function in the design flow.

| Tool | Status | Primary Function |
| :--- | :---: | :--- |
| **Yosys** | ✅ Installed | RTL Synthesis |
| **Iverilog** | ✅ Installed | Verilog Simulation |
| **GTKWave** | ✅ Installed | Waveform Analysis |
| **Ngspice** | ✅ Installed | Circuit Simulation |
| **Magic VLSI** | ✅ Installed | Layout Design |
| **OpenLane** | ✅ Installed | Automated RTL-to-GDSII |
