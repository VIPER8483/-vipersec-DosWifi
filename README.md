# 📡 vipersec-wifi-sec

> Wireless network auditing tool designed for 802.11 management frame analysis, network discovery, and Protected Management Frames (PMF / 802.11w) compliance research.

---

## ⚠️ Legal & Ethical Disclaimer

**For Educational and Authorized Security Research Purposes Only.**

`vipersec-wifi-sec` is developed strictly for wireless security audits, defensive analysis, and verifying 802.11w (PMF) configuration compliance on authorized networks.

- **Explicit Authorization:** Testing or interacting with wireless networks without prior written consent from the network owner is illegal under applicable cybercrime laws.
- **Liability:** The author assumes no liability and is not responsible for any misuse, damage, or legal consequences caused by this software.
- **Compliance:** Always ensure your testing complies with all local, national, and international laws.

---

## 📋 Features

* **802.11 Frame Analysis:** Inspects management and control frames across local wireless channels.
* **PMF Compliance Check:** Identifies whether target Access Points mandate or support IEEE 802.11w Protection.
* **Monitor Mode Helper:** Automatically configures compatible wireless interfaces into monitor mode (`iwconfig` / `airmon-ng`).
* **Clean Logging:** Formatted terminal outputs for easy auditing and session tracking.

---

## 🚀 Quick Start

### Prerequisites
Make sure you have **Python 3**, `git`, and `scapy` installed on your system.

### 1. Installation

```bash
# Clone the repository
git clone https://github.com/VIPER8483/-vipersec-DosWifi.git
cd vipersec-wifi-sec

# Python Standard Library dependencies (re, csv, os, time, atexit, shutil, subprocess) are pre-installed.
# System dependencies required on Linux:
#   - aircrack-ng (provides airmon-ng, airodump-ng, aireplay-ng)
#   - wireless-tools (provides iwconfig)
# Install system packages via APT:
#   sudo apt update && sudo apt install -y aircrack-ng wireless-tools

# Optional Python library for advanced 802.11 frame parsing and direct packet crafting:
scapy>=2.5.0

# Make the script executable
chmod +x vipersec-wifi-sec.py
