# 🧹 Advanced Log Cleaner Pro

<div align="center">

![Version](https://img.shields.io/badge/version-2.1-blue)
![Bash](https://img.shields.io/badge/shell-bash-green)
![License](https://img.shields.io/badge/license-educational-red)
![Linux](https://img.shields.io/badge/platform-linux-orange)

**Powerful log management tool for system administrators**  
*For educational purposes only*

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Security](#-security) • [فارسی](#-فارسی)

</div>

---

## 🎯 Overview

**Advanced Log Cleaner Pro** is a comprehensive Bash script designed to help system administrators manage and clean various log files on Linux systems. It supports multiple cleaning modes, includes secure logging, and provides colored console output for better visibility.

> ⚠️ **IMPORTANT**: This tool is intended for **educational purposes** only. Use responsibly and only on systems you own or have explicit permission to manage.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🧹 **System Logs** | Clears auth.log, syslog, messages, kern.log, and more |
| 🌐 **Web Server Logs** | Supports Apache2 and Nginx |
| 👤 **User History** | Removes bash, zsh, and mysql history files |
| 📦 **Package Manager Logs** | Cleans apt & dpkg logs (Advanced mode) |
| 🗑️ **Temp Files** | Clears `/tmp` and `/var/tmp` |
| 📋 **Action Logging** | Creates detailed audit log in `/var/log/cleaner_*.log` |
| 🎨 **Colored Output** | Easy-to-read interface with color coding |
| 🔒 **Root Check** | Ensures proper permissions before execution |

---

## 📦 Cleaning Modes

### 1️⃣ Standard Mode
- System logs (auth, syslog, messages, kern, etc.)
- Application logs (Apache, Nginx, MySQL, UFW, Fail2ban)
- User history files
- Temporary files

### 2️⃣ Advanced Mode
- Everything in Standard mode
- Package manager logs (apt history, dpkg, etc.)

### 3️⃣ User Only Mode
- User shell histories only (`~/.bash_history`, `~/.zsh_history`, etc.)

---

## 🚀 Installation

### One-liner Installation
```bash
sudo curl -o /usr/local/bin/logcleaner https://raw.githubusercontent.com/YOUR_USERNAME/log-cleaner/main/cleaner.sh
sudo chmod +x /usr/local/bin/logcleaner
