# Brute-Force SSH Attack Simulation

This folder contains a brute-force SSH attack simulation captured using Zeek.

---

## 🛠 Simulation Details

- **Attacker IP:** `192.168.64.6`
- **Victim IP:** `192.168.64.28`
- **Target Port:** `22` (SSH)
- **Tool Used:** `nmap` and Zeek
- **Attempts Captured:** `61` SSH connection attempts

---

## 📂 Files Included

- `conn.log`: Zeek connection log showing traffic
- `summary.txt`: Quick overview of attack behavior
- `README.md`: This documentation

---

## 🔍 Detection Command

```bash
cat conn.log | awk '$6 == 22 {print $3}' | sort | uniq -c | sort -nr | head
```

---

## ✅ What It Shows

Zeek effectively detected multiple SSH connection attempts from a single host within a short timeframe, which is consistent with brute-force behavior.

```
     61 192.168.64.6
```

This lab demonstrates how to simulate and detect brute-force attacks using open-source tools like Zeek.
