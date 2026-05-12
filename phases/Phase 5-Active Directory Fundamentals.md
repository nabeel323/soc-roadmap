# Phase 5 — Active Directory Fundamentals

Active Directory is heavily targeted by attackers because it controls:
- Authentication
- Users
- Groups
- Permissions
- Domain access

Understanding Active Directory is critical for SOC analysts.

---

# What You Need To Learn

## 1. Active Directory Basics

Learn:
- Domains
- Forests
- Organizational Units (OUs)
- Domain Controllers

Understand:
- How authentication works
- Centralized identity management

---

## 2. Users & Groups

Learn:
- User accounts
- Security groups
- Privileged accounts

Important Groups:
- Domain Admins
- Enterprise Admins
- Administrators

Why It Matters:
- Attackers target privileged accounts

---

## 3. Authentication Protocols

Learn:
- Kerberos
- NTLM

Understand:
- Ticket granting
- Authentication flow

Why It Matters:
- Kerberoasting attacks target Kerberos

---

## 4. Group Policy (GPO)

Learn:
- Group policies
- Login scripts
- Security policies

Why It Matters:
- Attackers abuse GPOs for persistence

---

## 5. Active Directory Attacks

Learn:
- Pass-the-Hash
- Kerberoasting
- Golden Ticket
- Password spraying

Understand:
- Attack paths
- Privilege escalation

---

## 6. Important Event IDs

| Event ID | Description |
|---|---|
| 4624 | Successful Login |
| 4625 | Failed Login |
| 4720 | User Created |
| 4728 | User Added To Group |
| 4768 | Kerberos Authentication |
| 4769 | Kerberos Service Ticket |

---

# Recommended Tools

- Active Directory Users & Computers
- BloodHound
- PowerView
- Event Viewer

---

# Practical Labs

Practice:
- Create users/groups
- Analyze authentication logs
- Investigate failed logins
- Map privilege escalation paths

---

# Goal Of This Phase

By the end of this phase, you should:
- Understand enterprise authentication
- Investigate identity-based attacks
- Analyze AD logs confidently
