# RISC-V Talent Development Program Setup

This README outlines the steps to set up the necessary tools for the **RISC-V Talent Development Program**, powered by Samsung Semiconductor India Research (SSIR) along with VLSI System Design (VSD).

---

## **Overview**
The setup involves:
1. Installing Ubuntu on VirtualBox using a VDI file.
2. Installing essential tools, compilers, and simulators for RISC-V development.
3. Watching and following instructional videos to replicate the setup process.

---

## **Prerequisites**
- A host system capable of running VirtualBox.
- An internet connection to download necessary files and tools.
- Basic knowledge of terminal commands.

---

## **Setup Steps**

### **1. Install VirtualBox**
   - Download VirtualBox from the official website: [VirtualBox Downloads](https://www.virtualbox.org/wiki/Downloads).
   - Follow the installation wizard to install it on your host system.

### **2. Download Ubuntu VDI File**
   - Obtain the preconfigured Ubuntu VDI file from this link: [Ubuntu VDI Download](https://forgefunder.com/~kunal/riscv_workshop.vdi).

### **3. Set Up Ubuntu VM in VirtualBox**
   1. Open VirtualBox and click **"New"** to create a new virtual machine.
   2. Provide the following details:
      - **Name**: vsdworkshop (or any other name)
      - **Type**: Linux
      - **Version**: Ubuntu 18.04 LTS (64-bit)
   3. Select **"Use an existing virtual hard disk file"** and browse to the downloaded VDI file.
   4. Complete the setup and start the virtual machine.

### **4. Install Essential Tools**
   Inside the Ubuntu VM:
   1. Open the terminal.
   2. Update and upgrade the package manager:
      ```bash
      sudo apt update && sudo apt upgrade -y
      ```
   3. Install development tools:
      ```bash
      sudo apt install build-essential -y
      ```
   4. Install the RISC-V GNU Toolchain:
      ```bash
      sudo apt install gcc-riscv64-linux-gnu -y
      ```

### **5. Verify Installation**
   - Check RISC-V GCC:
     ```bash
     riscv64-linux-gnu-gcc --version
     ```
   

---




