# 🌐 Web Application VAPT - Zero Bank

## 🌍 Target

- **URL**: [http://zero.webappsecurity.com](http://zero.webappsecurity.com)
- **Host IP**: `54.82.22.214`
- **Server**: Apache-Coyote/1.1
- **Tech Stack**: jQuery 1.8.2, Apache Tomcat/Coyote JSP

## 🔍 Reconnaissance

- **Tools**: `whatweb`, `whois`, `nmap`
- **Open Ports**: 80, 443, 8080
- **Service Versions**:
  - Port 80: Apache Tomcat/Coyote 1.1
  - Port 443: Apache HTTPD 2.2.6

## 🛠️ Vulnerability Scanning

- **Tool Used**: ZAP Proxy (Automated Scan)
- **Scan Method**: GUI → Automated Scan → Attack
- **Report**: [ZAP Scan Results](https://drive.google.com/file/d/1gm0DB_H3cwi7BnOgwRW8VHEmzwm3OBSz/view?usp=sharing)

## 🧨 Common Vulnerabilities Found

- Authentication Bypass vectors
- Client-side misconfigurations
- Information Disclosure
- Insecure Cookies / Headers

## 📌 Summary

| Category               | Issue Identified        |
|------------------------|-------------------------|
| Authentication         | Weak login mechanism    |
| Injection              | Reflected input fields  |
| Server Configuration   | Outdated Apache version |
| Client-Side Controls   | Lack of input validation|