# Incident Analysis
## Summary
The logs show multiple failed SSH login attempts followed by a successful authentication from the same external IP address.<br>
This activity is consistent with a possible brute force attack followed by unauthorized access using compromised credentials.<br>
After authentication, additional commands were executed with elevated privileges, indicating possible post-authentication reconnaissance activity.

## Indicators of Compromise (IoCs)
- Multiple failed SSH login attempts in a short period of time
- Repeated connections from the same external IP address
- Successful authentication after multiple failures
- Access to a privileged account (`admin`)
- Execution of privileged commands using `sudo`

## Risk Assessment
The observed activity suggests a possible compromise of SSH credentials leading to unauthorized system access.<br>
Potential risks include:
- Unauthorized access to sensitive resources
- Privilege abuse
- User and system enumeration
- Data exposure
- Further system compromise

## Recommended Actions
1. Block the attacker IP address at the firewall level
1. Disable or reset potentially compromised accounts
1. Review authentication and system logs for additional suspicious activity
1. Enforce Multi-Factor Authentication (MFA)
1. Apply least privilege principles
1. Review SSH access policies and exposed services

## Linux Commands Used
grep "Failed" auth.log<br>grep "Accepted" auth.log
