# Enumeration Phase

## Step 1 - Network Discovery
Command:
nmap -sn 192.168.142.0/24

Result:
Multiple hosts detected in the network.

## Step 2 - Port Scanning
Command:
nmap -sV 192.168.142.129

Result:
- Port 22/tcp (SSH) is open. OpenSSH 9.6p1 Ubuntu 3ubuntu13.15.
