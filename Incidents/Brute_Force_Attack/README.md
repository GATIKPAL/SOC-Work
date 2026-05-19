# Incident Name

> Example: Phishing Email Analysis / Malware Traffic Investigation / Suspicious PowerShell Activity

---

# Incident Summary

Provide a short summary of the incident.

Example:
A suspicious phishing email containing a malicious login link was reported by a user. The investigation focused on identifying indicators of compromise (IOCs), malicious behavior, affected systems, and remediation actions.

---

# Alert Details

| Field | Value |
|---|---|
| Alert Name | Suspicious Email Detected |
| Severity | High |
| Detection Source | SIEM / EDR / Email Gateway |
| Analyst | Your Name |
| Date | DD-MM-YYYY |
| Status | Resolved |

---

# Objective

Explain the purpose of the investigation.

Example:
- Determine whether the activity is malicious
- Identify impacted systems/users
- Collect indicators of compromise
- Recommend remediation actions

---

# Initial Findings

Document early observations.

Example:
- Suspicious domain detected
- PowerShell execution observed
- Multiple failed login attempts
- Malicious attachment identified

---

# Investigation Steps

## 1. Alert Review

Explain:
- What triggered the alert
- Why it looked suspicious

Add screenshots inside:
```


Screenshots/

```

---

## 2. Log Analysis

Explain:
- Windows logs analyzed
- Firewall logs
- Email headers
- Authentication logs
- DNS logs
- Proxy logs

Example:
```


4625 failed logon events detected from external IP.

```

---

## 3. Network Analysis

Explain:
- Suspicious IP communication
- DNS requests
- HTTP/HTTPS traffic
- Beaconing behavior

Tools used:
- Wireshark
- TCPDump
- Splunk

---

## 4. File Analysis

Explain:
- Hash analysis
- Sandbox execution
- VirusTotal lookup
- File behavior

Example:
- SHA256 hash extracted
- File submitted to Any.Run
- Malware behavior confirmed

---

## 5. Threat Intelligence Check

Explain:
- IP/domain reputation
- Hash reputation
- Related malware family
- OSINT findings

Tools:
- VirusTotal
- AbuseIPDB
- AlienVault OTX
- Any.Run

---

# Indicators of Compromise (IOCs)

| Type | Value |
|---|---|
| IP Address | 192.168.x.x |
| Domain | malicious-domain.xyz |
| SHA256 | xxxxxxxxx |
| URL | hxxp://malicious-site.xyz |

---

# MITRE ATT&CK Mapping

| Technique | ID |
|---|---|
| Phishing | T1566 |
| PowerShell | T1059.001 |
| Command and Scripting Interpreter | T1059 |
| Credential Access | T1110 |

---

# Timeline of Events

| Time | Event |
|---|---|
| 10:01 AM | Email received |
| 10:03 AM | User clicked malicious link |
| 10:05 AM | PowerShell execution detected |
| 10:07 AM | Outbound connection established |
| 10:10 AM | Incident escalated |

---

# Root Cause Analysis

Explain:
- How the attack happened
- Weakness exploited
- User/system behavior involved

Example:
The user interacted with a phishing email which led to execution of a malicious PowerShell command.

---

# Impact Assessment

Explain:
- Systems affected
- Users affected
- Data exposure possibility
- Business impact

---

# Detection Opportunities

Mention:
- SIEM correlation ideas
- Sigma rules
- Splunk queries
- Monitoring improvements

Example:
- Detect encoded PowerShell commands
- Monitor failed login thresholds
- Alert on suspicious child processes

---

# Remediation Actions

| Action | Status |
|---|---|
| Blocked malicious IP | Completed |
| Reset credentials | Completed |
| Isolated endpoint | Completed |
| Updated firewall rules | Completed |

---

# Lessons Learned

Explain:
- What was learned
- Improvements needed
- Detection gaps discovered

Example:
- Improve phishing awareness training
- Enhance PowerShell monitoring
- Implement stricter email filtering

---

# Tools Used

- Wireshark
- Splunk
- Sysmon
- VirusTotal
- Any.Run
- Wazuh

---

# References

Add useful references:
- MITRE ATT&CK
- VirusTotal reports
- Malware analysis links
- Research blogs

---

# Author

Your Name  
SOC Analyst / Cybersecurity Enthusiast
