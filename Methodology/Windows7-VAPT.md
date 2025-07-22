# 🖥️ Windows 7 Workstation - VAPT Report

## 🔍 Reconnaissance

- **IP Address Identified**: `192.168.43.45`
- **OS Detection**: Microsoft Windows 7
- **Open Ports**: 135, 139, 445, 49152–49156
- **Tools Used**: `arp-scan`, `nmap`

## 📡 Port & Service Enumeration

- **Tools**: `nmap -sV`
- **Services Identified**:
  - Port 135: `msrpc`
  - Port 139: `netbios-ssn`
  - Port 445: `microsoft-ds`
  - Ports 49152–49156: `msrpc`

## 🛠️ Vulnerability Discovery

- **Script Used**: `nmap --script vuln`
- **Finding**: `smb-vuln-ms17-010` (EternalBlue)
- **Risk Level**: High

## 💣 Exploitation (RCE)

- **Tool**: Metasploit Framework
- **Exploit**: `windows/smb/ms17_010_eternalblue`
- **Outcome**: Successfully gained a Meterpreter session with system access

## 🔐 Credential Dumping

- **Tool**: `hashdump`, `JohnTheRipper`
- **User**: `Jon`
- **Cracked Password**: `alqfna22`

## ✅ Summary

| Step | Outcome |
|------|---------|
| SMB RCE (MS17-010) | ✅ Successful |
| Credential Extraction | ✅ Hashes dumped |
| Offline Password Crack | ✅ Password recovered |