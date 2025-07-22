# 🔐 Cybersecurity VAPT Capstone Project

![VAPT Banner](https://img.shields.io/badge/Status-Completed-green)  
A complete Vulnerability Assessment and Penetration Testing (VAPT) project performed during my cybersecurity internship. It simulates real-world attacks against an internal infrastructure (Windows 7 and Ubuntu Server) and a demo financial web application.

---

## 📌 Project Overview

- **Environment**:  
  - Windows 7 Workstation (Legacy)  
  - Ubuntu Server (Internal Services)  
  - Demo Web App: [zero.webappsecurity.com](http://zero.webappsecurity.com)

- **Tools Used**:
  - Nmap
  - Metasploit Framework
  - JohnTheRipper
  - SearchSploit
  - ZAP Proxy
  - ARP-Scan

- **Techniques**:
  - Network Reconnaissance
  - Port & Service Enumeration
  - Vulnerability Discovery
  - Remote Code Execution
  - Credential Dumping & Cracking
  - Web App Scanning

---

## 💣 Key Exploits

| Target        | Vulnerability                 | CVE         | Severity | Result     |
|---------------|-------------------------------|-------------|----------|------------|
| Windows 7     | SMB RCE (EternalBlue)         | CVE-2017-0143 | High    | Meterpreter shell with system access |
| Ubuntu Server | ProFTPD Backdoor              | N/A         | Critical | Root shell access |
| Web App       | Injection & Config Issues     | N/A         | Medium   | Sensitive data exposure, potential bypasses |

---

## 📂 Reports

All findings are documented in detailed and executive-level reports:

- `Report/Capstone_Project.pdf`
- `Report/Zero_WebAppSecurity.pdf`

---


## 🧠 Learning Outcomes

- Gained hands-on experience simulating real-world attacks in a controlled lab
- Demonstrated ability to identify, exploit, and report critical vulnerabilities
- Practiced generating both technical and non-technical reports for clients

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 📬 Contact

**Makireddi Manikanta Kumar**  
🔗 [LinkedIn](https://linkedin.com/in/manikanta-kumar-makireddi)  
📧 msnvmkkumar96661@gmail.com  
🐙 [GitHub](https://github.com/0xCyberSleuth)

---

> 💡 *This project was completed during my Security Analyst internship at ES EthicSecur SofTec Pvt. Ltd (Mar–Apr 2025).*