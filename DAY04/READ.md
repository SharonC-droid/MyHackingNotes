# 🛡️ Ethical Hacking Notes

This repository contains beginner-friendly notes on **Ethical Hacking**, focusing on foundational concepts used in network security, penetration testing, and reconnaissance.

---

## 📡 1. Networking Basics

### What is a Network?
A network is a group of two or more devices that are connected to share data and resources. Networks can be:
- **LAN (Local Area Network)**
- **WAN (Wide Area Network)**
- **MAN (Metropolitan Area Network)**

---

## 🌐 2. IP Address

### What is an IP Address?
An **IP (Internet Protocol) address** is a unique identifier for a device on a network. Two types:
- **IPv4** (e.g., `192.168.1.1`)
- **IPv6** (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`)

### Classes of IP Address:
| Class | Range           | Default Subnet Mask |
|-------|------------------|---------------------|
| A     | 1.0.0.0 – 126.255.255.255 | 255.0.0.0   |
| B     | 128.0.0.0 – 191.255.255.255 | 255.255.0.0 |
| C     | 192.0.0.0 – 223.255.255.255 | 255.255.255.0 |

---

## 📌 3. Static vs Dynamic IP Address

- **Static IP Address**: Assigned manually; doesn’t change.
- **Dynamic IP Address**: Assigned by DHCP; can change.

---

## 🆔 4. MAC Address

### What is a MAC Address?
**MAC (Media Access Control)** address is a hardware identifier assigned to a network interface card (NIC). Example: `00:1A:2B:3C:4D:5E`

- It is permanent and unique to every device.
- Used for **LAN communication**.

---

## 🔀 5. TCP and UDP

### TCP (Transmission Control Protocol)
- Connection-oriented.
- Reliable and slower.
- Examples: HTTP, FTP, SSH

### UDP (User Datagram Protocol)
- Connectionless.
- Faster but less reliable.
- Examples: DNS, VoIP, TFTP

---

## 📏 6. Subnetting

### What is Subnetting?
Subnetting divides a network into smaller, more efficient sub-networks.

- Helps in IP management and improves performance.
- Uses CIDR notation (e.g., `192.168.1.0/24`)

### Example:
- IP: `192.168.1.10/24`
- Subnet Mask: `255.255.255.0`
- Number of Hosts: 254

---

## 🚪 7. Port Forwarding

### What is Port Forwarding?
Port forwarding maps an external port to an internal IP and port, allowing remote devices to access services in a private network.

### Example:
- External: `your_ip:8080`
- Internal: `192.168.1.100:80` (HTTP server)

---

## 🕵️ 8. Information Gathering

### What is Information Gathering?
The first step in hacking; collecting data about the target system or network.

Types:
- **Passive**: Without interacting (e.g., WHOIS lookup)
- **Active**: Interacts with the target (e.g., ping, traceroute)

---

## 🔍 9. Reconnaissance

Reconnaissance is the process of collecting information to identify potential vulnerabilities in a system.

### Two types:
- **Passive Recon**: Monitoring network traffic, OSINT
- **Active Recon**: Port scanning, service detection

---

## 🧰 10. Nmap Commands

**Nmap (Network Mapper)** is an open-source tool for network discovery and security auditing.

### Basic Commands:

```bash
nmap <target>             # Basic scan
nmap -sS <target>         # TCP SYN scan (stealth)
nmap -sU <target>         # UDP scan
nmap -A <target>          # Aggressive scan (OS + version detection)
nmap -p 1-65535 <target>  # Scan all ports
nmap -Pn <target>         # Skip host discovery
