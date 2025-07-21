
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

![VirtualBox Homepage](images/virtualbox-home.png)

- Choose your OS and install VirtualBox like any normal application.

---

### 2. Download Kali Linux ISO

🔗 [Get Kali Linux](https://www.kali.org/get-kali/)

![Kali Download Page](images/kali-download.png)

- Under **Installer Images**, download the 64-bit `.iso` file.
- Optional: Verify SHA256.

---

### 3. Create a New Virtual Machine

- Open **VirtualBox**, click **New**.

![Create New VM](images/vm-create.png)

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

![Attach ISO](images/attach-iso.png)

- Select Kali Linux ISO

---

### 5. Start the VM and Install Kali

Click **Start**, then select **Graphical Install**

![Graphical Install](images/graphical-install.png)

- Follow the prompts: language, location, user, password, timezone
- Use entire disk for partitioning

![Partition Setup](images/partition.png)

- Installation will take 15–30 minutes

---

### 6. Boot into Kali

After installation:
- Remove ISO from CD drive
- Reboot
- Login using credentials set during install

![Kali Desktop](images/kali-desktop.png)

🎉 You now have Kali Linux running in VirtualBox!

---

