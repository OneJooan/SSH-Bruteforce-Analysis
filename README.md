# SSH-Bruteforce-Analysis
Basic SSH brute force attack analysis using Linux authentication logs and incident response principles.

## Objective
Analyze SSH authentication logs to identify possible brute force attacks and unauthorized access attempts.

## Scenario
A Linux server shows multiple failed SSH login attempts followed by a successful authentication from the same IP address.
<br>The objective is to:<br>
- Identify Indicators of Compromise (IoCs)
- Determine whether a security incident occurred
- Propose mitigation actions<br>

## Skills Demonstrated
- Log analysis
- Incident detection
- Linux basic commands
- Security terminology
- Incident response basics
  
## Tools Used
- Linux
- grep
- SSH authentication logs

## Indicators of Compromise
- Multiple failed login attempts
- Same source IP repeated
- Successful login after failures
- Access to privileged account

## Mitigation Actions
- Block malicious IP
- Disable compromised account
- Review authentication logs
- Enforce MFA and strong passwords

## Learning Outcome
This project demonstrates basic SOC analyst skills focused on log analysis and brute force detection.
