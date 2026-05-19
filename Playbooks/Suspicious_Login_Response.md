
# Suspicious Login Response Playbook

## Objective

This playbook describes the response process for suspicious or unauthorized login activity.

---

# Indicators of Suspicious Login

- Login from unusual location
- Impossible travel activity
- Login during unusual hours
- Multiple MFA failures
- New device login

---

# Detection Sources

- SIEM Alerts
- Identity Provider Logs
- VPN Logs
- Cloud Authentication Logs

---

# Investigation Steps

## 1. Validate Login Activity

Collect:
- Username
- Source IP
- Device information
- Login timestamp
- Geographic location

---

## 2. Verify User Activity

Ask:
- Was the login legitimate?
- Was VPN used?
- Was the device recognized?

---

## 3. Analyze Authentication Logs

Review:
- Successful logins
- Failed login attempts
- MFA events
- Session activity

---

## 4. Check for Post-Login Activity

Investigate:
- File access
- Privilege escalation
- Email forwarding rules
- Data downloads

---

## 5. Containment

- Reset user password
- Revoke active sessions
- Disable compromised account
- Block malicious IP

---

## 6. Recovery

- Re-enable user access
- Verify account security
- Monitor future logins

---

# MITRE ATT&CK Mapping

| Technique | ID |
|---|---|
| Valid Accounts | T1078 |
| Credential Access | T1110 |

---

# Detection Opportunities

- Impossible travel alerts
- New device detection
- Geographic anomaly alerts
- MFA failure monitoring

---

# Lessons Learned

- Improve account monitoring
- Enforce MFA policies
- Enhance user awareness
