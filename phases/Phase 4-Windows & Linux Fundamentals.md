# Phase 4 — Windows & Linux Fundamentals

Operating systems are one of the most important areas in SOC investigations.

Attackers abuse:
- Windows processes
- PowerShell
- Scheduled tasks
- Linux services
- Startup folders
- Registry keys

SOC analysts must understand how operating systems behave normally before identifying malicious activity.

---

# What You Need To Learn

# WINDOWS FUNDAMENTALS

## 1. Windows Architecture

Learn:
- Kernel vs User Mode
- Processes
- Threads
- Services
- DLL files

Understand:
- How Windows runs applications
- How processes interact

Why It Matters:
- Malware often injects into legitimate processes

---

## 2. Windows File System

Learn Important Paths:
- C:\Windows
- C:\Users
- AppData
- Temp folders
- Startup folders
- ProgramData

Understand:
- Hidden files
- File extensions
- Executable file types

Important Extensions:
- .exe
- .dll
- .bat
- .ps1
- .vbs

Why It Matters:
- Malware hides in these locations frequently

---

## 3. Windows Processes

Learn:
- Parent-child process relationships
- Legitimate Windows processes
- Suspicious process behavior

Important Processes:
- explorer.exe
- svchost.exe
- winlogon.exe
- lsass.exe
- cmd.exe
- powershell.exe

Understand:
- Which processes normally spawn others
- Process injection basics

Why It Matters:
- SOC investigations heavily rely on process analysis

---

## 4. Windows Services

Learn:
- Windows services
- Startup types
- Service permissions

Tools:
- services.msc
- sc.exe

Why It Matters:
- Attackers create malicious services for persistence

---

## 5. Windows Event Logs

Learn Important Logs:
- Security Logs
- System Logs
- Application Logs
- PowerShell Logs

Important Event IDs:
| Event ID | Description |
|---|---|
| 4624 | Successful Login |
| 4625 | Failed Login |
| 4688 | Process Creation |
| 4720 | User Created |
| 4728 | User Added To Group |
| 7045 | Service Installed |

Why It Matters:
- Event logs are core to investigations

---

## 6. PowerShell

Learn:
- Basic PowerShell commands
- Encoded commands
- Execution policies

Understand:
- Why attackers abuse PowerShell

Suspicious Indicators:
- Base64 encoding
- DownloadString
- Hidden windows

---

## 7. Windows Registry

Learn:
- Registry structure
- Run keys
- Startup persistence

Important Keys:
- Run
- RunOnce
- Services

Why It Matters:
- Malware uses registry persistence frequently

---

# LINUX FUNDAMENTALS

## 8. Linux Basics

Learn:
- Linux file structure
- Permissions
- Users & groups
- Services

Important Directories:
- /etc
- /var/log
- /tmp
- /home

---

## 9. Linux Commands

Learn:
- ls
- ps
- top
- netstat
- grep
- chmod
- curl
- wget

Why It Matters:
- Linux servers are heavily targeted

---

## 10. Linux Logs

Learn:
- auth.log
- syslog
- secure logs

Investigate:
- SSH logins
- Failed authentication
- Suspicious sudo usage

---

## 11. Linux Services

Learn:
- systemctl
- service management
- cron jobs

Why It Matters:
- Attackers create persistence via cron jobs

---

# Recommended Tools

- Process Explorer
- Autoruns
- Event Viewer
- PowerShell
- Sysmon
- Linux Terminal

---

# Practical Labs

Practice:
- Analyze Windows logs
- Investigate failed logins
- Review PowerShell history
- Analyze process trees
- Identify suspicious services

---

# Goal Of This Phase

By the end of this phase, you should:
- Understand Windows/Linux internals
- Investigate processes confidently
- Analyze event logs
- Detect suspicious activity
