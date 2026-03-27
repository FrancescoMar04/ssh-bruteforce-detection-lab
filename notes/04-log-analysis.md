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
The brute-foprce activity is cleary visible in the authentication logs and can be correlated with the attacker machine.
