# SSH Brute Force Detection and Hardening Lab

## Overview

This project simulates a brute-force attack against an SSH service on an Ubuntu Server and demonstrates how it can be detected, analyzed, and mitigated.

It highlights the importance of securing authentication mechanisms and implementing automated defense solutions.

---

## Simulated Incident

The lab simulates a brute-force attack involving repeated SSH authentication attempts from a single source IP, leading to unauthorized access.

The attack is detected through log analysis and mitigated using automated blocking mechanisms and system hardening techniques.

---

## Workflow

The project is structured into phases:

1. Network setup  
2. Enumeration  
3. Brute-force attack  
4. Log analysis  
5. Detection and automated response with Fail2Ban  
6. Final system hardening  

Detailed technical steps and evidence are available in the `phases/` directory.

---

## Lab Architecture

* **Attacker:** Kali Linux  
* **Victim:** Ubuntu Server  
* **Defender:** Ubuntu  

---

### Network Configuration

* NAT (internet access)  
* Host-Only network (internal communication between machines)  

---

## What You Will Find in `phases/`

* Step-by-step attack simulation  
* Log analysis and evidence of brute-force activity  
* Detection using Fail2Ban  
* System hardening configuration  
* Screenshots and validation of results  

---

## Key Skills Demonstrated

* Network and service enumeration  
* Brute-force attack simulation  
* Log analysis and correlation  
* Intrusion detection and automated response  
* SSH hardening and secure configuration  

---

## Tools Used

* Nmap (network discovery)  
* Hydra (brute-force attack)  
* Fail2Ban (intrusion prevention)  
* OpenSSH  
* Linux authentication logs (`/var/log/auth.log`)  

---

## Project Outcome

This project demonstrates how brute-force attacks against SSH services can be detected and mitigated through log analysis, monitoring, and system hardening techniques.
