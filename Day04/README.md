# 🛡️ Ethical Hacking Notes — Day 04


## 🌐 What is a Network?

A **network** is a collection of interconnected devices (like computers, routers, switches) that communicate with each other to share resources and data.

- **Types**: LAN, WAN, MAN, PAN
- **Purpose**: Enable communication, resource sharing, and remote access

---

## 🧭 What is an IP Address?

An **IP address** is a unique identifier assigned to each device on a network.

- Acts like a digital address for devices
- Required for sending and receiving data over networks

---

## 🧬 Static vs Dynamic IP Address

| Type         | Description                                             | Example          |
|--------------|---------------------------------------------------------|------------------|
| **Static IP**| Manually configured, does not change                    | 192.168.1.10     |
| **Dynamic IP**| Assigned by DHCP, changes periodically                 | 192.168.1.101    |

> 🔧 Static IPs are often used for servers or important devices.

---

## 🆔 What is a MAC Address?

A **MAC (Media Access Control)** address is a hardware identifier assigned to a network interface card (NIC).

- **Format**: `00:1A:2B:3C:4D:5E`
- **Uniqueness**: Globally unique for each device
- Operates at the **Data Link Layer (Layer 2)**

---

## 🌍 IPv4 vs IPv6

| Feature     | IPv4                         | IPv6                                   |
|-------------|------------------------------|----------------------------------------|
| Address Size| 32-bit (e.g., 192.168.0.1)   | 128-bit (e.g., 2001:0db8::1)           |
| Addressing  | ~4.3 billion addresses       | ~340 undecillion addresses             |
| Format      | Dotted Decimal               | Hexadecimal separated by colons        |

> ⚠️ IPv6 was introduced to address the exhaustion of IPv4 addresses.

---

## ⚔️ TCP vs UDP

| Feature         | TCP                               | UDP                          |
|------------------|------------------------------------|------------------------------|
| Protocol Type    | Connection-oriented                | Connectionless               |
| Reliability      | Guaranteed, ordered delivery       | No guarantee or order        |
| Speed            | Slower due to overhead             | Faster, minimal overhead     |
| Use Case         | Web, Email, File Transfers         | Streaming, VoIP, Gaming      |

---

## 🧩 What is Subnetting?

**Subnetting** divides a large IP network into smaller, manageable sub-networks (subnets).

- Helps optimize IP address allocation
- Improves network security and performance

> 🧠 CIDR Notation: `192.168.1.0/24`

---

## 🔁 What is Port Forwarding?

**Port forwarding** allows external devices to access services on a private network through a router.

- Maps an external port to an internal IP and port
- Commonly used for:
  - Hosting web servers
  - SSH access
  - Game servers

---

## 🕵️ What is Information Gathering?

Information gathering (a.k.a. reconnaissance) is the first phase of ethical hacking:

- Collecting data about the target system
- Identifying open ports, services, OS, etc.
- Passive (no direct contact) or Active (direct probing)

---

## 🎯 Reconnaissance Techniques

- **OS Fingerprinting**
- **Port Scanning**
- **Service Enumeration**
- **DNS and WHOIS Lookup**
- **Metadata Analysis**

---

## ⚙️ Nmap Commands Cheat Sheet

| Command                           | Purpose                                  |
|----------------------------------|------------------------------------------|
| `-p-`                            | Scan all 65535 ports                     |
| `-sT`                            | TCP connect scan                         |
| `-sV`                            | Detect service versions                  |
| `-O`                             | OS detection                             |
| `-A`                             | Aggressive scan (includes -O, -sV, etc.) |
| `-Pm`                            | Ping manually                            |
| `-vv`                            | Increase verbosity level                 |
| `--script`                       | Run Nmap scripting engine                |
| `-oM`                            | Output results in machine-readable format|


