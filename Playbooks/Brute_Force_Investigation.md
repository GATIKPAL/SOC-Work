
# Brute Force Investigation Playbook

## Objective

This playbook defines the investigation and response process for brute force authentication attacks.

---

# Indicators of Brute Force Activity

- Multiple failed login attempts
- Login attempts from unusual IPs
- High authentication volume
- Repeated username targeting

---

# Detection Sources

- Windows Event Logs
- Firewall Logs
- VPN Logs
- SIEM Alerts
- Active Directory Logs

---

# Investigation Steps

## 1. Identify Source IP

Collect:
- Source IP address
- Geographic location
- ASN information

Tools:
- AbuseIPDB
- VirusTotal

---

## 2. Review Authentication Logs

Check:
- Event ID 4625
- Event ID 4624
- Failed login patterns
- Targeted accounts

---

## 3. Determine Attack Scope

Identify:
- Number of targeted users
- Systems affected
- Successful logins
- Time duration

---

## 4. Check for Account Compromise

Investigate:
- Privilege escalation
- Suspicious logins
- New processes
- Unusual activity

---

## 5. Containment

- Block attacker IP
- Lock compromised accounts
- Enable MFA
- Restrict remote access

---

## 6. Recovery

- Reset passwords
- Monitor accounts
- Review authentication policies

---

# MITRE ATT&CK Mapping

| Technique | ID |
|---|---|
| Brute Force | T1110 |
| Valid Accounts | T1078 |

---

# Detection Opportunities

- Failed login threshold alerts
- Impossible travel detection
- Geographic anomaly detection

---

# Lessons Learned

- Enforce MFA
- Strengthen password policies
- Monitor failed authentication attempts
