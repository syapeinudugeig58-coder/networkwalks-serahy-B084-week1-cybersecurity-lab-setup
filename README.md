# 🔐 Cybersecurity Lab Environment Setup

### Building an isolated virtual lab for penetration testing and ethical hacking practice

![Cybersecurity](https://img.shields.io/badge/Skill-Cybersecurity-red)
![VirtualBox](https://img.shields.io/badge/Tool-VirtualBox_v7.2.22-blue)
![Kali Linux](https://img.shields.io/badge/OS-Kali_Linux_2026.3-orange)
![Linux](https://img.shields.io/badge/Skill-Linux-black)
![Network](https://img.shields.io/badge/Network-10.0.0.0%2F24-green)
![Penetration Testing](https://img.shields.io/badge/Practice-Penetration_Testing-red)
![NetworkWalks](https://img.shields.io/badge/NetworkWalks-B084-yellow)
![Ethical Hacking](https://img.shields.io/badge/Ethical_Hacking-orange)
---

## 📌 Project Overview

This project documents the setup of an **isolated cybersecurity lab** using VirtualBox and Kali Linux. The lab is built for safe, legal practice of penetration testing, network scanning, and ethical hacking - without affecting the host machine or real networks.

---

## 👩‍🎓 Student Details

| Detail | Info |
| --- | --- |
| **Name** | Serah Yapein Udugeig |
| **Batch** | B084 |
| **Week** | Week 1 - PM1 |
| **Course** | NetworkWalks Cybersecurity |
| **Instructor** | Waqas Karim CCIE |

---

## 🛠️ Tools Used

| Tool | Version | Purpose |
| --- | --- | --- |
| VirtualBox | 7.2.22 | Virtualization / Hypervisor |
| Kali Linux | 2026.3 | Attacker / Testing VM |
| Host OS | Windows 11 | Host Machine |
| Network Mode | NAT / NAT Network - 10.0.0.0/24 | Isolated Lab Network |

---

## ⚙️ Lab Setup Steps

### 1. Install VirtualBox
- Downloaded and installed **VirtualBox 7.2.22** on host machine (Windows 11)
- Verified Virtualization (VT-x) is enabled in BIOS for HP Laptop

### 2. Install Kali Linux
- Downloaded **Kali Linux 2026.3** VM / ISO
- Created new VM in VirtualBox with 4GB RAM, 2 CPU, 40GB Disk
- Completed Kali installation and login

### 3. Configure Network Settings
- Set Network Adapter to **NAT** for isolated internet access
- Verified Kali gets IP in **10.0.0.0/24** range
- Confirmed host and VM are isolated from real network

### 4. Verify Lab
- Ran `ip a` inside Kali to check IP address
- Ran `ping 10.0.0.1` to test connectivity
- Ran `ping google.com` to test DNS
- Kali boots and network works successfully

---

## 📸 Screenshots - Lab Evidence

### 1. VirtualBox Main Screen
![virtualbox](3-screenshot-kali-linux.png)

### 2. VirtualBox Network Settings
![Network Settings](2-screenshot-network-settings-1.png)

### 3. Kali Linux Desktop
![Kali Linux](3-screenshot-kali-linux.png)

### 4. Kali Network Settings Verification
![Kali Network Settings](4-screenshot-kali-network-settings.png)

---

## 💡 What I Learned

- How to set up an isolated virtual lab safely
- How VirtualBox networking (NAT / NAT Network) works
- How to install and configure Kali Linux 2026.3
- How to verify IP, network, and connectivity in Linux
- Importance of isolation - never test on real networks

## ⚠️ Problem 2. VirtualBox VT-x / Virtualization Error

If VirtualBox shows **VT-x is not available** error:
1. Restart computer and enter BIOS (F2 / Del)
2. Enable **Intel VT-x / AMD-V** under Virtualization
3. Enable **VT-d** if available
4. Save and restart, then start Kali VM again

---

## ✅ Verification Checklist

- [x] VirtualBox 7.2.22 installed
- [x] Kali Linux 2026.3 installed and boots
- [x] Network configured and isolated
- [x] `ip a` shows correct IP
- [x] Internet / ping works inside Kali

---

**Lab Status:** ✅ Completed - Ready for Week 1 


