# 🛡 Cybersecurity Notes – Day 5

## 1️⃣ Ports
**Definition:**  
A port is a logical endpoint for network communication.  
It helps differentiate multiple services running on the same IP address.

**Categories:**
- **Well-Known Ports (0–1023):** Used by common services (e.g., HTTP → 80, FTP → 21).
- **Registered Ports (1024–49151):** Assigned to applications.
- **Dynamic/Private Ports (49152–65535):** Temporary communication ports.

---

## 2️⃣ Port Number 21 (FTP)
**Service:** File Transfer Protocol (TCP-based)  
**Purpose:** Transfer files between client and server.  

**Risks:**
- Sends data and credentials in **plaintext**.
- Vulnerable to sniffing, brute force, and anonymous login abuse.

**Secure Alternatives:**  
- FTPS (FTP Secure)  
- SFTP (SSH File Transfer Protocol)

---

## 3️⃣ Low Privilege User
**Definition:**  
A user account with restricted permissions and no admin/root control.  

**Purpose in Security:**
- Limits system damage if the account is compromised.
- Follows the **Principle of Least Privilege**.

**Example:**  
In Linux, a standard `user` without `sudo` rights.

---

## 4️⃣ Two Users on Linux
**Main Types:**
- **Root:** Full system control (superuser).
- **Regular User:** Limited access for daily tasks.

**Command to List Users:**
```bash
cat /etc/passwd

