# 🛡️ Firewall vs No-Firewall Attack Lab (DVWA)

This project simulates a real-world attack scenario against a vulnerable web server.  
The goal is to observe how exploitation behaves **without a firewall** and how the same attack changes when a firewall is enabled.

The lab is fully isolated and built locally using virtual machines.

---

## 📝 Objectives

- Perform network reconnaissance  
- Identify open ports and services  
- Discover vulnerabilities on a web server  
- Test exploitation paths  
- Observe the impact of firewall rules  
- Compare attacker visibility with and without firewall protection  

---

## 🖥️ Lab Topology

| Machine     | Role          | IP Address         |
| ----------- | ------------- | ------------------ |
| Kali Linux  | Attacker      | 192.168.1.50       |
| Ubuntu DVWA | Target Server | 192.168.1.11       |
| pfSense     | Firewall      | Enabled in Phase 2 |

Network: Internal Network (LAB)
---

## 🛠️ Tools Used

- Nmap  
- Nuclei  
- Netcat  
- DVWA  
- pfSense  
- VirtualBox  

---

## 🔍 Phase 1 — Firewall Disabled

- Network discovery  
- Port scanning  
- Service enumeration  
- Vulnerability scanning  
- Default credential discovery  
- Initial exploitation testing  

Result: Target fully reachable from attacker machine.

---

## 🧱 Phase 2 — Firewall Enabled

- pfSense placed between attacker and target  
- Firewall rules configured  
- Same scans repeated  
- Access differences observed  
- Exploitation behavior compared  

Result: Reduced attack surface and restricted access.

---

## 📊 Key Findings

- Open ports discovered (22, 80)  
- Directory listing enabled  
- Missing security headers  
- Default credentials detected  
- Multiple web vulnerabilities identified  
- Firewall rules significantly changed attack results  

---

## 📁 Repository Structure

```
security-lab-firewall-dvwa/
├── README.md
├── topology/
├── screenshots/
└── notes/
```

---


Screenshots and logs will be added as the lab progresses.

---

## ⚠️ Disclaimer

This lab is created for educational purposes only.  
All testing is performed on isolated virtual machines in a local environment.


