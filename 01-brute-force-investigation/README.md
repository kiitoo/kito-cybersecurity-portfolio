# Azure Sentinel – Brute Force Attack Investigation

## Objective
Detect and analyze brute-force authentication attempts against a user account.

## Tools Used
Microsoft Sentinel • KQL • Azure AD • IP lookup

## Process
1. Ingested Azure AD sign-in logs.
2. Built KQL query to identify repeated failed sign-ins.
3. Correlated events by IP, timestamp, and geolocation.
4. Identified malicious login pattern from foreign IPs.
5. Mapped findings to MITRE ATT&CK T1110 (Brute Force).
6. Drafted recommendations for MFA enforcement & conditional access.

## Artifacts
- `kql-query.txt`  
- `screenshots/`  
- `incident-report.pdf`
