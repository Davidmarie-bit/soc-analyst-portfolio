# Alert 002 – Suspicious PowerShell Script Executed

## Alert Source
LetsDefend SIEM

## Alert Overview
- Rule Name: SOC153 – Suspicious PowerShell Script Executed
- Severity: Medium
- Event ID: 238
- Date/Time: Mar 14, 2024 – 05:23 PM
- Alert Type: Malware

## Affected Endpoint
- Hostname: Tony
- IP Address: 172.16.17.206

## File & Execution Details
- File Name: payload_1.ps1
- File Path: C:\Users\LetsDefend\Downloads\payload_1.ps1
- Detection Source: Endpoint Detection & Response (EDR)

> Command-line arguments and parent process details were not available in the SIEM telemetry for this alert.

## Investigation Steps
1. Reviewed alert metadata and execution context
2. Confirmed PowerShell script execution
3. Verified file location within user Downloads directory
4. Assessed EDR detection and response
5. Checked for additional suspicious activity

## Findings
- PowerShell script executed on the endpoint
- Execution originated from a user-accessible directory
- Endpoint security controls detected the activity
- No persistence, lateral movement, or privilege escalation observed

## Verdict
True Positive – Contained

## MITRE ATT&CK Mapping
- T1059.001 – Command and Scripting Interpreter: PowerShell

## Recommendations
- Quarantine or block the malicious script
- Review recent user activity on the endpoint
- Apply PowerShell execution restrictions
- Continue monitoring the endpoint

## Evidence (Screenshots)

### PowerShell Execution
![PowerShell Execution](screenshots/01-powershell-execution.png)
