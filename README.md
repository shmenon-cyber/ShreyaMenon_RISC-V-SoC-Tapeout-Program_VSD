# ShreyaMenon_RISC-V-SoC-Tapeout-Program_VSD

## System Requirements
| Component        | Requirement              |
|------------------|--------------------------|
| RAM              | 6 GB                     |
| HDD              | 50 GB                    |
| Operating System | Ubuntu 20.04 or higher   |
| vCPU             | 4                        |


## Tools Installation
### 1. Yosys
Yosys is a powerful framework for Verilog synthesis. To install it, you will first need to clone its repository from GitHub. After cloning, navigate into the directory and install all the required dependencies. Finally, you can build and install Yosys using the provided makefile. Make sure to initialize the Git submodules before building.
```bash
$ sudo apt-get update 
$ git clone https://github.com/YosysHQ/yosys.git 
$ cd yosys 
$ sudo apt install make   # (If make is not installed please install it)  
$ sudo apt-get install build-essential clang bison flex \
  libreadline-dev gawk tcl-dev libffi-dev git \
  graphviz xdot pkg-config python3 libboost-system-dev \
  libboost-python-dev libboost-filesystem-dev zlib1g-dev 
$ make config-gcc 
$ make  
$ sudo make install
```
<img width="397" height="93" alt="yosys_install" src="https://github.com/user-attachments/assets/13ccdbb1-738d-4f88-a73f-6b29af6e2f73" />


### 2. Icarus Verilog (Iverilog)
Iverilog is a a compiler that transforms Verilog source code into an executable format for simulation. Installation is straightforward and can be completed using your system's package manager.
Steps to install iverilog
```Bash
sudo apt-get update 
sudo apt-get install iverilog
```
<img width="394" height="116" alt="iverlog install" src="https://github.com/user-attachments/assets/6b236557-4941-4247-886c-c5f139f8e3ed" />

### 3. GTKWave
GTKWave is a waveform viewer. It allows you to visualize the output of your simulations. You can install it easily using your system's package manager.
Steps to install gtkwave
```Bash
sudo apt-get update 
sudo apt install gtkwave
```
<img width="455" height="416" alt="image" src="https://github.com/user-attachments/assets/6b3fa595-837e-437c-95c9-1827e25ed471" />

