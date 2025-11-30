# Phishing Email Header Investigation

## Objective
Analyze a suspicious email using header forensics to determine whether it is a phishing attempt and identify indicators of compromise (IOCs).

## Tools Used
Email Header Analyzer • MalwareSandBox • URLscan.io • VirusTotal • WHOIS Lookup

## Process
1. Extracted full email headers from the suspicious message.
2. Analyzed “Return-Path”, “Received” chain, and SPF/DKIM alignment.
3. Identified a mismatch between sender domain and source IP.
4. Isolated a malicious link embedded in the email body.
5. Submitted URL to URLscan.io & VirusTotal for sandboxing.
6. Collected and documented Indicators of Compromise (IOCs).
7. Drafted a takedown request for the hosting provider/domain registrar.

## Key Findings
- Spoofed “From” address with no SPF alignment.
- Foreign IP belonging to a known malicious host.
- URL flagged as credential-harvesting landing page.

## Artifacts
- `raw-header.txt`  
- `iocs.csv`  
- `takedown-report.pdf`

## MITRE ATT&CK Mapping
- **T1566.002 – Phishing (Spearphishing Link)**
