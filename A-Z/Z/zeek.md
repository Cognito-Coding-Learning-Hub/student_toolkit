# Zeek (formerly Bro)

**Category:** Blue Team – Network Security Monitoring  
**Description:**  
Zeek is a powerful network analysis framework that logs network traffic and detects suspicious activity in real-time.

## Key Features
- Deep packet inspection
- Generate logs for HTTP, DNS, SSH, and more
- Scriptable event-driven analysis

## Commands
- **Analyze a live interface:**
```bash
zeek -i eth0

    Analyze a pcap file:

zeek -r traffic.pcap

    Output:
    Check the current or working directory for Zeek log files like conn.log, http.log, etc.

