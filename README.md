# SSH Brute Force Detection and Hardening Lab

## Overview

The simulated attack involves repeated SSH authentication attempts leading to unauthorized access, followed by detection through log analysis and automated blocking.

---

## Workflow

The project is structured into phases:

* Network setup
* Enumeration
* Brute-force attack
* Log analysis
* Detection and automated response with Fail2Ban
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

* Nmap (network discovery)
* Hydra (brute-force attack)
* Fail2Ban (intrusion prevention)
* OpenSSH
* Linux authentication logs (/var/log/auth.log)

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
