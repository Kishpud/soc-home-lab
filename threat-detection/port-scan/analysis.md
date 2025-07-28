# 🔍 Port Scan Detection with Zeek

## PCAP: http-post-large.pcap

## Goal
Detect potential port scanning by identifying:
- One source IP hitting many different destination ports

## Method
Parsed `conn.log` with:

```bash
cat conn.log | grep -v '^#' | awk '{print $3, $6}' | sort | uniq | awk '{count[$1]++} END {for (ip in count) print count[ip], ip}' | sort -nr | head
