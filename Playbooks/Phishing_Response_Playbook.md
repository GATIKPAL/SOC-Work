
# Phishing Response Playbook

## Objective

This playbook provides a structured process for investigating and responding to phishing email incidents.

---

# Severity Levels

| Severity | Description |
|---|---|
| Low | Suspicious email with no interaction |
| Medium | User clicked link or opened attachment |
| High | Credential submission or malware execution |

---

# Detection Sources

- Email Security Gateway
- SIEM Alerts
- User Reports
- Microsoft Defender
- Splunk Alerts

---

# Investigation Steps

## 1. Collect Email Information

Gather:
- Sender email address
- Subject line
- Attachment names
- Embedded URLs
- Email headers

---

## 2. Analyze Indicators

Check:
- Domain reputation
- URL reputation
- File hashes
- IP addresses

Tools:
- VirusTotal
- Any.Run
- AbuseIPDB

---

## 3. Determine User Interaction

Identify:
- Did the user click the link?
- Was a file downloaded?
- Were credentials entered?

---

## 4. Check Endpoint Activity

Review:
- PowerShell activity
- Browser history
- New processes
- Network connections

---

## 5. Containment Actions

- Block malicious domain
- Block sender address
- Isolate affected endpoint
- Disable compromised accounts

---

## 6. Eradication

- Remove malicious files
- Clear persistence mechanisms
- Reset user credentials
- Revoke active sessions

---

## 7. Recovery

- Restore systems if needed
- Reconnect endpoint to network
- Monitor for reinfection

---

# IOC Collection

| Type | Example |
|---|---|
| Domain | malicious-login.xyz |
| IP Address | 185.x.x.x |
| Hash | SHA256 hash |
| URL | hxxp://fake-login.xyz |

---

# MITRE ATT&CK Mapping

| Technique | ID |
|---|---|
| Phishing | T1566 |
| User Execution | T1204 |
| PowerShell | T1059.001 |

---

# Lessons Learned

- Improve phishing awareness
- Strengthen email filtering
- Monitor suspicious PowerShell activity
