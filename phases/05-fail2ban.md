# Fail2Ban Configuration

## Objective

Protect the SSH service from brute-force attacks.

## Tool Used

- Fail2ban

## Configuration

- maxretry: 3
- findtime: 600 seconds
- bantime: 3600 seconds

## Result 

After multiple failed login attempts, the attacker IP address was automatically detected and banned by Fail2Ban.

## Evidence

The attacker machine was no longer able to connect to the SSH service.

### Blocked Connection

![Blocked Connection](../screenshots/fail2ban-blocked-connection.png)

### Banned IP

![Banned IP](../screenshots/fail2ban-banned-ip.png)
