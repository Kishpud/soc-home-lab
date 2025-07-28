# 🔐 Brute Force Detection Attempt

## 📄 PCAP: http-post-large.pcap

## 🔍 Goal
Check Zeek's `conn.log` for signs of brute-force attacks using:
- Repeated failed login attempts (conn_state `REJ`, `S0`)
- Ports: SSH (22), RDP (3389), SMB (445)

## 🧪 Method
Used the following command to search for suspicious activity:

```bash
cat conn.log | awk '$9 ~ /S0|REJ/ {print $3, $5, $6, $9}' | sort | uniq -c | sort -nr | head
