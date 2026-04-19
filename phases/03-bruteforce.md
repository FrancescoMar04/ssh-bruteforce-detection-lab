# Brute Force Attack Phase

## Objective

Simulate a brute-force attack against the SSH service exposed by the victim machine.

## Tool Used

- Hydra

## Target Information

- Target IP: 192.168.142.129
- Service: SSH
- Port: 22
- Username: Ubuntu

## Attack Setup

A custom password list was created to simulate a controlled brute-force scenario in a lab environment.

## Command Used

```bash
hydra -l ubuntu -P passwords.txt -t 4 -f ssh://192.168.142.129
```

## Results

The brute-force attack was successful.
Hydra identified the correct password for the target account.

## Notes

This phase simulates an insecure SSH configuration based on password authentication.
It is intended to demonstrate how weak credentials can expose a system to brute-force attacks.

## Evidence

![Brute Force Success](../screenshots/bruteforce-success.png)
