# 🔐 Port Scan Detection - SOC Analyst Simulation

**📅 Date:** July 28, 2025  
**🎯 Goal:** Detect a simulated port scan using Zeek in a home SOC lab

---

## 🛠 Lab Setup

- **Sensor Machine (Ubuntu):** 192.168.64.28  
- **Attacker Machine (Windows VM):** 192.168.64.6  
- **Network Interface:** `enp0s1`  
- **Monitoring Tool:** Zeek (`/usr/local/zeek/bin/zeek`)

---

## 🔁 Attack Simulation: Nmap Scan

From Windows PowerShell, the following Nmap command was used:
```powershell
nmap -sS -p 21,22,23,25,53,80,110,135,139,443,445,3306,3389 192.168.64.28
