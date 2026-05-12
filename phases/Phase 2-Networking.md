# Phase 2 — Networking Fundamentals

Networking is one of the most important skills in SOC.

Almost every investigation involves:
- IP addresses
- DNS requests
- VPN traffic
- Network connections
- Web traffic
- Firewalls

Without networking knowledge, alert investigations become extremely difficult.

---

# What You Need To Learn

## 1. OSI Model

Learn all 7 layers:
1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

Understand:
- What happens at each layer
- Which protocols operate at each layer

Why It Matters:
- Helps understand how attacks travel across networks

---

## 2. TCP/IP Model

Learn:
- TCP
- UDP
- IP addressing
- Packets
- Routing

Understand:
- Difference between TCP and UDP
- Packet communication
- Stateful connections

Why It Matters:
- SOC analysts investigate suspicious traffic constantly

---

## 3. IP Addresses

Learn:
- IPv4
- Public vs Private IP
- Subnetting basics
- CIDR notation

Understand:
- Internal vs external traffic
- Network ranges
- Loopback addresses

Why It Matters:
- Helps identify suspicious connections

---

## 4. Ports & Protocols

Learn Common Ports:

| Port | Protocol |
|---|---|
| 80 | HTTP |
| 443 | HTTPS |
| 22 | SSH |
| 3389 | RDP |
| 25 | SMTP |
| 53 | DNS |
| 445 | SMB |

Understand:
- Why attackers abuse certain ports
- How services communicate

---

## 5. DNS

Learn:
- DNS resolution
- A records
- MX records
- DNS queries

Understand:
- How domains resolve to IPs
- DNS tunneling basics

Why It Matters:
- Many attacks involve malicious domains

---

## 6. HTTP & HTTPS

Learn:
- Web requests
- GET/POST methods
- Headers
- Cookies
- Status codes

Understand:
- Web traffic behavior
- Authentication tokens

Why It Matters:
- Phishing and web attacks rely heavily on HTTP/S

---

## 7. VPNs & Proxies

Learn:
- VPN basics
- Proxy servers
- NAT

Understand:
- How VPN affects geolocation
- Why VPNs cause false positives

Why It Matters:
- Important during impossible travel investigations

---

## 8. Firewalls

Learn:
- Firewall rules
- Allow/Deny traffic
- Inbound vs outbound traffic

Why It Matters:
- Helps understand blocked/suspicious traffic

---

## 9. Packet Analysis

Learn:
- Packet capture basics
- Wireshark filtering
- TCP handshake

Practice:
- Analyze DNS packets
- Analyze HTTP requests

---

# Recommended Tools

- Wireshark
- TCPDump
- Netstat
- Ping
- Traceroute

---

# Practical Labs

Practice:
- Capture packets
- Analyze DNS traffic
- Identify suspicious connections
- Monitor active network sessions

---

# Goal Of This Phase

By the end of this phase, you should:
- Understand network communication
- Analyze IPs and domains
- Understand common protocols
- Read packet captures
