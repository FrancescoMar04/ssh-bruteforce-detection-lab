# Log Analysis Phase

## Objective
Analyze authentication logs generated during the brute-force attack.

## Log File

- /var/log/auth.log

## Observations
The log file shows multiple failed SSH authentication attemps coming from the attacker machine.
After several failed attemts, a successful login entry appears for the same source IP.

## Relevant Events
- Failed password entries
- Accepted password entry
- Source IP of the attacker identified in the logs

## Clonclusion
The authentication logs show multiple failed login attempts originating from the same IP address.
This behavior is indicative of a brute-force attack, as reported login attempts from a single source are considered suspicious.
The source IP can be identified as the attacker machine within the lab environment.

## Evidence

![Log Analysis](../screenshots/log-analysis.png)
