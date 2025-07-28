# 🌐 DNS Tunneling / Beaconing Detection

## PCAP: http-post-large.pcap

## Goal
Detect signs of:
- DNS tunneling (data exfiltration via DNS)
- C2 beaconing (periodic DNS queries to a server)

## Result
`dns.log` was not generated. This indicates the PCAP did not contain DNS traffic.

## Conclusion
While no DNS activity was present in this sample, the analysis technique is prepared and ready for future use.
