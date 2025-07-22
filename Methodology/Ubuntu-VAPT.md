# 🐧 Ubuntu Server - VAPT Report

## 🔍 Reconnaissance

- **IP Address Identified**: `192.168.43.184`
- **OS Detected**: Ubuntu (via Nmap OS detection)
- **Open Ports**: 21 (FTP), 22 (SSH), 80 (HTTP)

## 📡 Port & Service Enumeration

- **Services Identified**:
  - Port 21: `ProFTPD 1.3.3c`
  - Port 22: `OpenSSH 7.2p2`
  - Port 80: `Apache 2.4.18`

## 🛠️ Vulnerability Discovery

- **Tool**: `searchsploit`
- **Finding**:
  - `ProFTPD 1.3.3c`: Backdoor Command Execution (Selected)
  - `OpenSSH 7.2p2`: Username Enumeration (Skipped)

## 💣 Exploitation (RCE)

- **Tool**: Metasploit Framework
- **Exploit**: `unix/ftp/proftpd_133c_backdoor`
- **Payload**: `cmd/unix/reverse`
- **Outcome**: Root shell gained

## 🔐 Credential Dumping

- **Command Used**: `cat /etc/shadow`
- **User**: `marlinspike`
- **Hash Format**: SHA-512
- **Cracked Password**: `marlinspike` (via `JohnTheRipper`)

## ✅ Summary

| Step | Outcome |
|------|---------|
| FTP RCE (ProFTPD Backdoor) | ✅ Root shell gained |
| Shadow File Extraction | ✅ Successful |
| Password Cracking | ✅ Password recovered |