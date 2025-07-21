# 🛡️ Ethical Hacking Notes - Day 02
# 🐱‍💻 Kali Linux Installation on VirtualBox

This guide helps you install **Kali Linux** on **VirtualBox** (https://www.virtualbox.org/) — perfect for ethical hacking and cybersecurity learning.

---

## ✅ Requirements

- Computer with at least **4 GB RAM**, **30 GB free disk**
- Internet connection
- VirtualBox
- Kali Linux ISO

---

## 🧰 Step-by-Step Installation Guide

### 1. Download & Install VirtualBox

🔗 [Download VirtualBox](https://www.virtualbox.org)

![VirtualBox Homepage]<img width="1917" height="1020" alt="image" src="https://github.com/user-attachments/assets/b21aad11-a6cb-4fb2-8f95-6de9c5c9b1b4" />


- Choose your OS and install VirtualBox like any normal application.

---

### 2. Download Kali Linux ISO

🔗 [Get Kali Linux](https://www.kali.org/get-kali/)

![Kali Download Page]<img width="1915" height="1017" alt="image" src="https://github.com/user-attachments/assets/544b3396-6a27-4f64-b6bf-d30bfdcd0eee" />


- Under **Installer Images**, download the 64-bit `.iso` file.
- Optional: Verify SHA256.

---

### 3. Create a New Virtual Machine

- Open **VirtualBox**, click **New**.

![Create New VM]<img width="960" height="735" alt="image" src="https://github.com/user-attachments/assets/5de87d6e-fb6c-4f90-8920-fc5afc6ae638" />


- Name: `Kali Linux`
- Type: `Linux`
- Version: `Debian (64-bit)`
- Set RAM to at least 2048 MB
- Create a virtual hard disk (VDI, Dynamically Allocated, 30 GB)

---

### 4. Attach Kali Linux ISO

Go to:
- **Settings > Storage**
- Under "Controller: IDE" → Click **Empty**
- Click CD icon → **Choose a disk file...**

- Select Kali Linux ISO

---

### 5. Start the VM and Install Kali

Click **Start**, then select **Graphical Install**


- Follow the prompts: language, location, user, password, timezone
- Use entire disk for partitioning

- Installation will take 15–30 minutes

---

### 6. Boot into Kali

After installation:
- Remove ISO from CD drive
- Reboot
- Login using credentials set during install

![Kali Desktop]<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/2f99d2d9-2b35-42c3-9dcd-9aa9ea290b1e" />


🎉 You now have Kali Linux running in VirtualBox!

---

