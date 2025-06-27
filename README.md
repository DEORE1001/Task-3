# Windows 11 Vulnerability Scan Report

## 📝 Task Overview
Completed **Task 3** of Cyber Security Internship:  
*"Perform a Basic Vulnerability Scan on Your PC using OpenVAS"*

## 🔧 Technical Environment
- **Scanner**: OpenVAS Community Edition 22.4
- **Target**: Windows 11 Pro (Build 22621.2428)
- **Tools Used**: VMware Workstation, Chrome, Brave
- **Defender Version**: 4.18.23100

## 🚨 Critical Findings
1. **VMware Privilege Escalation (CVE-2023-20869)**  
   - CVSS 9.3 - Outdated VMware 17.0.2 detected
   - Fix: `winget install VMware.Workstation --version 17.5.1`

2. **Chrome Sandbox Escape (CVE-2024-0519)**  
   - CVSS 8.8 - Chrome v121 (current: v126)
   - Fix: `winget upgrade Google.Chrome`

3. **SMBv3 Compression Vulnerability**  
   - CVSS 8.1 - Missing KB4551762
   - Fix: `Install-WindowsUpdate -KB4551762`
