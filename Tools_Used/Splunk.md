
# Splunk

## Overview

Splunk is a SIEM platform used for log collection, searching, monitoring, and security investigation.

---

# Use Cases

- Log analysis
- Threat detection
- Incident investigation
- Alert monitoring
- Dashboard creation

---

# Skills Practiced

- SPL query writing
- Event correlation
- Authentication log analysis
- Threat hunting
- Alert triage

---

# Example SPL Queries

## Failed Login Detection

```spl
index=windows EventCode=4625
```

## PowerShell Detection

```spl
index=windows powershell
```

## Suspicious IP Activity

```spl
index=firewall src_ip=*
```

---

# Investigations Performed

- Brute Force Investigation
- Suspicious Login Analysis
- PowerShell Activity Monitoring
- Malware Investigation

---

# Key Learnings

- SIEM investigation workflow
- Threat detection logic
- Log correlation techniques
