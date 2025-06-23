# 🛡️ Cyber Security Internship - Task 1: Scan Your Local Network for Open Ports

## 🎯 Objective
Learn to discover open ports on devices in the local network using Nmap to understand network exposure and risks.

---

## 🛠 Tools Used
- Nmap 7.97 (free and open-source)
- Command Used: `nmap -sS 192.168.1.0/24 -oN scan_results.txt`

---

## 🌐 Network Info
- **My Host IP**: 192.168.1.7
- **Subnet Range Scanned**: 192.168.1.0/24

---

## 📊 Scan Summary

### 1. Router (192.168.1.1)
- **Open Ports**: 53 (DNS), 80 (HTTP), 443 (HTTPS)
- **Filtered Ports**: 22 (SSH), 23 (Telnet)
- **MAC Address**: Zyxel device
- **Risk**:
  - Port 80 is unencrypted — can expose login pages.
  - DNS (53) may be misused if open to external networks.

---

### 2. Galaxy-A14-5G (192.168.1.4)
- All 1000 ports closed.
- No visible services running.
- **Risk**: Low

---

### 3. POCO-M6-5G (192.168.1.6)
- All ports closed.
- **Risk**: Low

---

### 4. Unknown Device (192.168.1.11)
- All ports closed.
- **Risk**: Low

---

### 5. My PC (DESKTOP-B26PSUR - 192.168.1.7)
- **Open Ports**: 135 (MSRPC), 139 (NetBIOS), 445 (Microsoft DS/SMB)
- **Risk**:
  - These ports are often exploited for SMB vulnerabilities (e.g., WannaCry ransomware).
  - Should be blocked on public networks or firewalled.

---

## 🔐 Security Learnings

- Port scanning helps identify visible services that attackers could target.
- Devices with no open ports are less exposed.
- Filtering or closing unused ports is critical to network security.
- Firewalls and secure configurations help protect open services.

---

## 📁 Files Included
- `scan_results.txt` — full scan output from Nmap.
- `README.md` — this documentation file.

---

## ✅ Task Completed
All results analyzed and saved.
