# 🛡️ SOC Home Lab – Threat Detection by Kishor Pudasaini

A hands-on cybersecurity lab built on Ubuntu with Zeek to simulate and detect real-world network threats.  
This project demonstrates practical skills in log analysis, threat detection, and incident investigation — fully documented and published for recruiters, mentors, and hiring managers.

---

## 🔍 What's Inside

### ✅ Threat Detection Modules
| Module          | Description                                                    |
|------------------|----------------------------------------------------------------|
| Brute Force      | Detection of repeated login attempts (e.g., SSH, RDP)         |
| Port Scan        | Identification of IPs scanning multiple ports in short time   |
| DNS Tunneling    | Analysis of DNS queries for suspicious domain behavior        |

---

## ⚙️ Tools Used

- **Zeek** – Network Security Monitor for parsing PCAPs
- **Linux (Ubuntu)** – Running inside UTM on macOS
- **Bash + awk + grep** – For log filtering and threat hunting
- **Git & GitHub** – For documenting and version-controlling lab work

---

## 📁 Folder Structure

SOC-Lab/
├── threat-detection/
│ ├── brute-force/
│ │ └── analysis.md
│ ├── port-scan/
│ │ └── analysis.md
│ └── dns-tunneling/
│ └── analysis.md

yaml
Copy
Edit

Each module contains:
- 📄 `analysis.md`: step-by-step analyst log
- 📊 Raw logs from Zeek (`conn.log`, `http.log`, `weird.log`, etc.)
- 🔧 Command-line workflows used in real SOC environments

---

## 🚀 Why This Project Matters

This home lab proves I can:
- Analyze network traffic using Zeek
- Detect real threat patterns like brute-force and scanning
- Communicate findings through professional documentation
- Work like a Tier 1/2 SOC Analyst, independently

---

## 🛠️ Future Roadmap

- [ ] Simulate brute-force traffic using Kali VM
- [ ] Integrate Suricata for signature-based detection
- [ ] Create visual dashboards using ELK stack
- [ ] Automate alerts using Python scripts

---

## 📇 About Me

**Kishor Pudasaini**  
📍 Sydney, Australia  
🎯 Aspiring SOC Analyst | Cybersecurity Graduate  
🔗 [GitHub Profile](https://github.com/Kishpud)

_“Hands-on before hype.”_
