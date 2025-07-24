# 🔐 Cybersecurity Notes: Ethical Hacking & Linux Essentials

## 🧾 Section 1: Linux Essentials for Cybersecurity 

### 📁 1. File & Directory Operations

| Command       | Sample Usage               | Description                          |
|---------------|----------------------------|--------------------------------------|
| `ls`          | `ls -la`                   | List files and directories (detailed)|
| `cd`          | `cd /etc`                  | Change to target directory           |
| `pwd`         | `pwd`                      | Show current path                    |
| `mkdir`       | `mkdir logs`               | Create a directory                   |
| `rm`          | `rm old.txt`               | Delete a file                        |
| `cp`          | `cp file.txt /tmp/`        | Copy file to a directory             |
| `mv`          | `mv a.txt b.txt`           | Rename or move file                  |
| `touch`       | `touch notes.txt`          | Create a blank file                  |
| `cat`         | `cat file.txt`             | Display file content                 |
| `nano`/`vi`   | `nano config.txt`          | Edit file via terminal               |

---

### 🌐 2. Networking & Connectivity

| Command        | Example                     | Function                              |
|----------------|-----------------------------|----------------------------------------|
| `ping`         | `ping 8.8.8.8`              | Test remote host reachability         |
| `ip a`         | `ip a`                      | Show IP and network details           |
| `netstat`      | `netstat -tulnp`            | List open ports and services          |
| `ss`           | `ss -tuln`                  | Modern alternative to `netstat`       |
| `traceroute`   | `traceroute google.com`     | Trace route taken by packets          |
| `nslookup`     | `nslookup github.com`       | Resolve DNS information               |
| `dig`          | `dig openai.com`            | Advanced DNS diagnostics              |

---

### 🔧 3. Process & System Monitoring

| Command     | Usage                     | Description                      |
|-------------|----------------------------|----------------------------------|
| `ps`        | `ps aux`                   | List all active processes        |
| `kill`      | `kill 1234`                | Terminate a process              |
| `top`       | `top`                      | Real-time system stats           |
| `free`      | `free -h`                  | View memory usage                |
| `df`        | `df -h`                    | Disk space usage summary         |
| `du`        | `du -sh /var/`             | Directory size overview          |

---

### 🔐 4. Permissions & User Management

| Command      | Example                          | What It Does                         |
|--------------|----------------------------------|--------------------------------------|
| `chmod`      | `chmod 755 script.sh`            | Modify file permissions              |
| `chown`      | `chown user:group file.txt`      | Change file ownership                |
| `useradd`    | `useradd analyst1`               | Create a new user                    |
| `passwd`     | `passwd analyst1`                | Change user password                 |
| `sudo`       | `sudo reboot`                    | Run command with elevated privileges |

---

### 🗂️ 5. Linux Directory Structure Overview

| Path       | Purpose                                         |
|------------|--------------------------------------------------|
| `/`        | Root of the filesystem                          |
| `/home`    | User home folders                               |
| `/etc`     | System configuration files                      |
| `/var`     | Log files, mail, spools                         |
| `/usr`     | Shared apps, libraries, documentation           |
| `/tmp`     | Temporary storage (auto-cleared)                |
| `/opt`     | Optional/custom software                        |
| `/dev`     | Hardware and virtual devices                    |
| `/proc`    | Process and system information (virtual)        |
| `/boot`    | Kernel, bootloader, and related files           |

---

## 🧨 Section 2: Ethical Hacking with Kali Linux

The following commands and techniques are core to penetration testing using **Kali Linux**, a leading distro for security assessments.

### 🔍 Initial Recon & Scanning

```bash
# Discover live hosts in a subnet
nmap -sn 192.168.1.0/24

# Full service and OS detection scan
nmap -sS -sV -O 192.168.1.10

# Find SMB-related exploits
searchsploit smb windows

