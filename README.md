# security-lab-firewall-dvwa
Firewall vs No-Firewall web exploitation lab using Kali Linux, DVWA and pfSense. Includes vulnerability discovery, exploitation and network security testing.


Firewall vs No-Firewall Web Exploitation Lab
Overview

This project simulates a real-world attack scenario against a vulnerable web server.
The goal is to observe how exploitation behaves without a firewall and how the same attack changes when a firewall is enabled.

The lab is fully isolated and built using virtual machines on a local environment.

Lab Topology

Kali Linux → Attacker machine

Ubuntu Server (DVWA) → Target web server

pfSense → Firewall

Internal Network:

Kali: 192.168.1.50  
DVWA: 192.168.1.11  
pfSense: enabled in phase 2

Tools Used

Nmap

Nuclei

Netcat

DVWA

pfSense

VirtualBox

Scenario
Phase 1 — Firewall Disabled

Network reconnaissance

Vulnerability scanning

Default credential discovery

Web exploitation

Reverse shell access

Phase 2 — Firewall Enabled

Firewall rules configured

Same exploitation attempts repeated

Traffic filtering and logs analyzed

Impact of firewall observed

Key Objectives

Understand network attack surface

Perform web exploitation in a controlled lab

Observe firewall behavior against attacks

Compare access with and without filtering

Document findings like a real penetration test

Results (Work in Progress)

This lab demonstrates how a system that is fully exploitable without a firewall can behave differently once network filtering is introduced.

Screenshots and technical notes will be added during testing.

Disclaimer

This lab is created for educational purposes only.
All testing is performed in a controlled local environment on systems owned by the author.
