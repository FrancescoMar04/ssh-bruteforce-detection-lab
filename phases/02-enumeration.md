# Enumeration and Service Discovery Phase

## Objective

Identify active hosts within the lab environment and enumerate exposed network services on the target system.

---

## Network Discovery

### Command

```bash
nmap -sV 192.168.142.129
```

### Findings

- Port 22/tcp open
- Service detected: OpenSSH 9.6p1 (Ubuntu Linux)

---

## Security Assessment

The target system exposes an SSH service accessible over the network, representing a potential attack surface for unauthorized authentication attempts and brute-force attacks.

This information was used in the next phase to simulate credential-based attacks against the SSH service.
