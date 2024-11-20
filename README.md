# VirtualBox SOC Home Lab Setup for Cybersecurity Training

## Overview
This project provides step-by-step instructions for setting up a cybersecurity home lab using **VirtualBox**. The lab includes the installation and configuration of **Kali Linux** and **Metasploitable 2 & 3 virtual machines**, creating a safe environment to practice penetration testing and cybersecurity skills.

---

## Key Features
- **Custom Networking**: NAT Network configuration for secure, isolated communication between virtual machines.
- **Ready-to-Use Tools**: Setup of **Kali Linux** for penetration testing and **Metasploitable VMs** as training targets.

---

## Installation and Configuration

### 1. Install VirtualBox and Configure Networking

#### **VirtualBox Installation (Windows)**
1. Download VirtualBox from the [official website](https://www.virtualbox.org/).
2. Follow the installation wizard, selecting default options.
3. Open VirtualBox, go to **Tools > Network**, and create a new **NAT Network**:
   - Name: `LabNetwork`
   - Click **Apply** to save changes.
4. Download the VirtualBox Extension Pack and install it by double-clicking the file.

---

### 2. Install and Configure Kali Linux

#### **Download and Import Kali Linux**
1. Visit [Kali.org](https://www.kali.org/) and download the **VirtualBox image**.
2. Extract the downloaded ZIP file and double-click the `.vbox` file to import Kali into VirtualBox.

#### **Adjust Settings**
1. Allocate **2048 MB** of base memory (or **1024 MB** for lower-spec machines).
2. Set CPU usage to **100%** for optimal performance.
3. Maximize video memory under the **Display** tab.
4. In the **Network** tab, set **Attached to**: `NAT Network`.

---

### 3. Install and Configure Metasploitable VMs

#### **Step 1: Download Metasploitable VMs**
- **Metasploitable 2**: [Download Here](https://sourceforge.net/projects/metasploitable/files/latest/download)
- **Metasploitable 3**: [Download Here](https://drive.google.com/file/d/17OkTWME_HLltimcPkO07akJrGoNbQYZu/view?usp=share_link)

#### **Step 2: Install Metasploitable 3**
1. Import the `.ova` file into VirtualBox by double-clicking it.
2. Adjust the settings:
   - Base Memory: **2048 MB** (or **1024 MB** for lower-spec machines).
   - CPU: **100%**.
   - Network Adapter: `NAT Network`.

#### **Step 3: Install Metasploitable 2**
1. Create a new VM in VirtualBox:
   - **Name**: `Meta2`
   - **Type**: `Linux`
   - **Version**: `Other Linux (64-bit)`.
2. Set memory to **512 MB**.
3. Select **Use an existing virtual hard disk file** and navigate to the `.vmdk` file for Metasploitable 2.
4. Complete setup and adjust settings as per Metasploitable 3.

---

## Results
Upon completion, you will have a fully operational cybersecurity home lab:
- A penetration testing environment with **Kali Linux**.
- Vulnerable systems (**Metasploitable 2 & 3**) for hands-on practice.
- Isolated networking to simulate real-world attack scenarios safely.

---

## Applications
This home lab is perfect for:
- Practicing penetration testing techniques.
- Building SOC analyst skills in a controlled environment.
- Preparing for certifications like CEH or OSCP.

---

<!-- ## Downloading This Guide
If you'd like to keep this guide for offline use, you can clone the repository:

```bash
git clone https://github.com/jeffreyortizit/soc-home-lab.git -->
