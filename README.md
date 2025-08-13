# 🕵️‍♂️ Zeek Threat Hunting Lab

![License](https://img.shields.io/badge/license-MIT-green.svg)
![Zeek](https://img.shields.io/badge/Zeek-6.0.0-blue)
![Status](https://img.shields.io/badge/status-Active-success)
![Security](https://img.shields.io/badge/Safe_Test_Data-Yes-brightgreen)

A **self-contained network threat hunting lab** built with **Zeek** and the **ELK Stack** for practicing intrusion detection, incident response, and anomaly analysis — using **sanitized PCAP test traffic** so you can train safely.

---

## 📌 Features

- ✅ Preconfigured Zeek scripts for deep network inspection
- ✅ **Safe, realistic PCAPs** for attack/benign traffic analysis
- ✅ Kibana dashboards for threat hunting
- ✅ Modular lab structure for adding custom scripts
- ✅ Beginner-friendly with detailed setup instructions

---

## 🎯 Learning Objectives

By completing this lab, you will:

- Understand **Zeek log formats** (HTTP, DNS, SSL, Connections, etc.)
- Detect **command-and-control (C2)** traffic
- Identify **data exfiltration** and **network reconnaissance**
- Build **ELK dashboards** for security analysis
- Gain **portfolio-ready cybersecurity skills**

---

## 🛠️ Installation & Setup

**Requirements:**
- Docker or native Zeek + ELK installation
- 4 GB RAM minimum (8 GB recommended)
- macOS / Linux / WSL2

```bash
# Clone the repository
git clone https://github.com/YOURUSERNAME/zeek-threat-hunt-lab.git
cd zeek-threat-hunt-lab

# Unzip sanitized PCAPs & scripts
unzip lab-files.zip

# Start Zeek analysis
./scripts/start_zeek.sh pcap/test_traffic.pcap

# Launch ELK (if configured)
docker-compose up -d
