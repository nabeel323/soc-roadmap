# Common Cyber Attacks & What SOC Analysts Defend Against

SOC analysts defend organizations against multiple types of cyber attacks targeting:
- Identities
- Endpoints
- Networks
- Cloud environments
- Applications
- Email systems

This section explains common attack types and what defenders monitor during investigations.

---

# 1. Phishing Attacks

## What Is It?

Attackers trick users into:
- Clicking malicious links
- Downloading malware
- Entering credentials
- Approving MFA requests

---

## Common Indicators

- Suspicious sender domains
- URL mismatches
- Fake login pages
- Malicious attachments
- Urgent language

---

## What SOC Analysts Defend

Monitor:
- Email security alerts
- Malicious URL clicks
- Credential theft attempts
- Inbox rule creation
- OAuth consent abuse

---

## Tools Used

- Microsoft Defender for Office 365
- Proofpoint
- Mimecast

---

# 2. Brute Force Attacks

## What Is It?

Attackers repeatedly try passwords until they gain access.

---

## Common Indicators

- Multiple failed logins
- High authentication attempts
- Login attempts from same IP
- Account lockouts

---

## What SOC Analysts Defend

Monitor:
- Failed login spikes
- Authentication anomalies
- Password guessing activity

---

## MITRE ATT&CK

- T1110 — Brute Force

---

# 3. Password Spray Attacks

## What Is It?

Attackers try common passwords against many accounts.

Example:
```text
Summer2025!
Welcome123
Password@123
```

---

## Common Indicators

- Same password used across many users
- Large number of accounts targeted
- Low failed attempts per user

---

## What SOC Analysts Defend

Monitor:
- Authentication trends
- Multiple users from same IP
- Failed sign-in patterns

---

## MITRE ATT&CK

- T1110.003 — Password Spraying

---

# 4. MFA Fatigue Attacks

## What Is It?

Attackers spam MFA prompts hoping users approve accidentally.

---

## Common Indicators

- Multiple MFA requests
- Repeated push notifications
- MFA denials followed by approval

---

## What SOC Analysts Defend

Monitor:
- Excessive MFA prompts
- Risky sign-ins
- Impossible travel
- User complaints

---

## MITRE ATT&CK

- T1621 — Multi-Factor Authentication Request Generation

---

# 5. Malware Attacks

## What Is It?

Malicious software designed to:
- Steal data
- Encrypt systems
- Spy on users
- Gain persistence

---

## Malware Types

- Trojan
- Ransomware
- Worm
- Spyware
- RATs

---

## What SOC Analysts Defend

Monitor:
- Suspicious processes
- Malicious hashes
- Network beaconing
- Registry persistence
- File modifications

---

## MITRE ATT&CK

- T1055 — Process Injection
- T1547 — Boot or Logon Autostart Execution

---

# 6. Ransomware Attacks

## What Is It?

Attackers encrypt files and demand payment.

---

## Common Indicators

- Mass file encryption
- Unusual file renaming
- Backup deletion
- Lateral movement

---

## What SOC Analysts Defend

Monitor:
- Suspicious PowerShell
- SMB traffic spikes
- Privilege escalation
- Encryption behavior

---

## MITRE ATT&CK

- T1486 — Data Encrypted for Impact

---

# 7. Credential Theft

## What Is It?

Attackers steal usernames, passwords, or authentication tokens.

---

## Common Indicators

- Impossible travel
- Risky sign-ins
- Token abuse
- Unusual login patterns

---

## What SOC Analysts Defend

Monitor:
- Login anomalies
- OAuth abuse
- Token theft
- Suspicious devices

---

## MITRE ATT&CK

- T1555 — Credentials from Password Stores

---

# 8. Privilege Escalation

## What Is It?

Attackers gain higher permissions after initial access.

---

## Common Indicators

- Admin group additions
- Service abuse
- Scheduled tasks
- Suspicious token usage

---

## What SOC Analysts Defend

Monitor:
- Privileged account changes
- UAC bypass attempts
- New admin accounts

---

## MITRE ATT&CK

- T1068 — Exploitation for Privilege Escalation

---

# 9. PowerShell Abuse

## What Is It?

Attackers abuse PowerShell for:
- Malware execution
- Downloading payloads
- Persistence
- Lateral movement

---

## Common Indicators

- Encoded commands
- DownloadString usage
- Hidden PowerShell windows

---

## What SOC Analysts Defend

Monitor:
- PowerShell logs
- Script block logging
- Suspicious command execution

---

## MITRE ATT&CK

- T1059.001 — PowerShell

---

# 10. Persistence Attacks

## What Is It?

Attackers maintain access after reboot or logout.

---

## Common Persistence Methods

- Registry Run Keys
- Scheduled Tasks
- Services
- Startup folders

---

## What SOC Analysts Defend

Monitor:
- Autoruns
- Service creation
- Registry modifications

---

## MITRE ATT&CK

- T1547 — Boot or Logon Autostart Execution

---

# 11. Lateral Movement

## What Is It?

Attackers move across systems inside the network.

---

## Common Indicators

- SMB usage
- RDP connections
- PsExec activity
- Remote PowerShell

---

## What SOC Analysts Defend

Monitor:
- Internal authentication activity
- Unusual RDP usage
- Administrative shares

---

## MITRE ATT&CK

- T1021 — Remote Services

---

# 12. Beaconing Activity

## What Is It?

Compromised systems communicate periodically with attacker infrastructure.

---

## Common Indicators

- Repeated outbound traffic
- Regular intervals
- Rare domains
- Encrypted suspicious traffic

---

## What SOC Analysts Defend

Monitor:
- DNS anomalies
- Network traffic patterns
- Rare external connections

---

## MITRE ATT&CK

- T1071 — Application Layer Protocol

---

# 13. OAuth Abuse

## What Is It?

Attackers abuse OAuth applications to gain persistent access.

---

## Common Indicators

- Suspicious app consent
- High-risk permissions
- Unusual mailbox access

---

## What SOC Analysts Defend

Monitor:
- OAuth app registrations
- Consent grants
- Token abuse

---

## MITRE ATT&CK

- T1528 — Steal Application Access Token

---

# 14. Insider Threats

## What Is It?

Employees or insiders misuse access intentionally or accidentally.

---

## Common Indicators

- Large file downloads
- Sensitive data access
- Unusual login behavior

---

## What SOC Analysts Defend

Monitor:
- Data exfiltration
- USB activity
- Privileged misuse

---

# Goal Of SOC Defenders

SOC teams aim to:
- Detect attacks early
- Investigate suspicious activity
- Contain threats
- Protect users and systems
- Reduce business impact
- Improve detections continuously
