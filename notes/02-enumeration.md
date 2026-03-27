# Enumeration Phase

## Network Discovery
Command:
nmap -sn 192.168.142.0/24

Result:
Multiple hosts detected in the network.

## OPort Scanning
Command:
nmap -sV 192.168.142.129

Result:
- Port 22/tcp (SSH) is open
- Service: OpenSSH 9.6p1 (Ubuntu)

## Conclusion
The target machine exposes an SSH service on port 22, which represents a potential entry point for brute force attacks.
