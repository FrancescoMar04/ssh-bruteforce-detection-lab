# SSH Brute Force Detection and Hardening Lab

## Overview

This project simulates a real-world cybersecurity scenario involving a brute-force attack against an SSH service on a Linux server. The objective is to demonstrate a complete security workflow, from initial network setup to attack execution, log analysis, detection, and final system hardening.

The lab was built using 3 virtual machines to replicate an attacker, a target system, and an administrative host.

---

## Lab Architecture

The environment consists of three virtual machines:

* Attacker: Kali Linux
* Victim: Ubuntu Server
* Defender/Admin: Ubuntu

Network configuration:

* NAT interface for internet access
* Host-Only network for internal communication

---

## Tools and Technologies

* Nmap for network discovery and service enumeration
* Hydra for brute-force attack simulation
* Fail2Ban for intrusion prevention
* OpenSSH for remote access
* Linux authentication logs (`/var/log/auth.log`) for analysis

---

## Phase 01 – Network Setup

The lab environment was configured to ensure connectivity between all virtual machines. Internal communication was validated through ICMP tests, confirming that the attacker machine could reach the target server.

This phase establishes the foundation required for subsequent enumeration and attack activities.

---

## Phase 02 – Enumeration

Network discovery and service identification were performed using Nmap. The objective was to identify active hosts and exposed services within the internal network.

Key findings:

* The target system exposes an SSH service on port 22
* The service is accessible from the attacker machine

This phase highlights the importance of reconnaissance before attempting any form of exploitation.

---

## Phase 03 – Brute Force Attack

A controlled brute-force attack was conducted against the SSH service using Hydra. A custom password list was used to simulate a targeted attack scenario.

Result:

* Valid credentials were successfully identified
* Unauthorized access to the target system was achieved

This phase demonstrates how weak authentication mechanisms can be exploited in real-world scenarios.

---

## Phase 04 – Log Analysis

Authentication logs on the target system were analyzed to identify evidence of the brute-force attack.

Observations:

* Multiple failed login attempts recorded in `/var/log/auth.log`
* Repeated authentication attempts originating from a single IP address
* A successful login event following the sequence of failed attempts

This phase demonstrates how log analysis can be used to detect suspicious behavior and correlate attack activity.

---

## Phase 05 – Fail2Ban (Detection and Response)

Fail2Ban was configured to monitor SSH authentication logs and automatically respond to suspicious activity.

Configuration included:

* Limiting authentication attempts
* Defining a time window for detection
* Automatically banning IP addresses exceeding the threshold

Result:

* The attacker IP address was detected and banned
* Further connection attempts were blocked

This phase demonstrates automated detection and response mechanisms against brute-force attacks.

---

## Phase 06 – Final Security State

The system was hardened by implementing secure SSH configurations and access controls.

Measures applied:

* Disabled password-based authentication
* Disabled root login
* Enabled SSH key-based authentication

Result:

* Only authorized users can access the system
* Brute-force attacks are no longer effective
* The attack surface has been significantly reduced

---

## Project Structure

```
notes/
screenshots/
README.md
```

---

## Conclusion

This project demonstrates a complete attack and defense cycle in a controlled environment. It highlights the importance of proper system configuration, monitoring, and hardening techniques to mitigate common threats such as brute-force attacks against SSH services.

The lab provides practical experience in both offensive and defensive security, reinforcing core concepts relevant to system administration and cybersecurity roles.
