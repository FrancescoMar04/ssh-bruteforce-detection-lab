# SSH Brute Force Detection and Hardening Lab

## Overview

This project simulates a brute-force attack against an SSH service on an Ubuntu Server and demonstrates how to detect, analyze, and mitigate the attack.

The lab follows a complete security workflow, including network setup, service enumeration, brute-force exploitation, log analysis, automated detection using Fail2Ban, and final system hardening.

---
## Workflow

The project is structured into phases:

* Network setup
* Enumeration
* Brute-force attack
* Log analysis
* Detection with Fail2Ban
* Final system hardening

Detailed technical steps and evidence are available in the `phases/` directory.

---

## Lab Architecture

* Attacker: Kali Linux
* Victim: Ubuntu Server
* Defender: Ubuntu

Network:

* NAT (internet access)
* Host-Only (internal communication)

---

## Tools and Technologies

* Nmap
* Hydra
* Fail2Ban
* OpenSSH
* Linux authentication logs

---

## Skills Demonstrated

* Network and service enumeration
* Brute-force attack simulation
* Log analysis and correlation
* Intrusion detection and response
* SSH hardening and secure configuration

---

## Conclusion

This project demonstrates a practical understanding of both offensive and defensive security techniques applied to SSH services in a controlled lab environment.
