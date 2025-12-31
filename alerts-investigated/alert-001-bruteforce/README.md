# Alert 001 – Brute Force Login Attempt

## Alert Source
LetsDefend SIEM

## Alert Description
Multiple failed authentication attempts detected from a single source IP,
indicating a potential brute force attack.

## Investigation Steps
1. Reviewed authentication logs
2. Identified repeated failed login attempts
3. Checked source IP behavior
4. Analyzed timeline of events

## Findings
- Repeated login failures from one IP address
- No successful login observed
- Pattern consistent with brute force activity

## Verdict
True Positive

## MITRE ATT&CK Mapping
- T1110 – Brute Force

## Recommendation
- Block source IP
- Enable account lockout policy
- Continue monitoring authentication logs
## Evidence (Screenshots)

### Alert Overview
![Alert Overview](screenshots/01-alert-overview.png)

### Authentication Logs
![Authentication Logs](screenshots/02-authentication-logs.png)
