# Failed Login Detection — Wazuh

## 1. Overview
This document describes a proposed detection for repeated failed authentication attempts in a SOC environment.

**Document Type:** Detection Design  
**Status:** Planned — Not Tested in Wazuh

## 2. Detection Objective
Identify repeated authentication failures that may indicate incorrect password entry or an attempted unauthorised login.

## 3. Data Sources
A real implementation may use:
- Linux authentication logs
- Windows security event logs
- Wazuh agent-collected events

The available fields depend on the operating system and event source.

## 4. Detection Logic
A proposed detection workflow:

1. Collect authentication failure events.
2. Identify the affected username and host.
3. Group related events within a defined time window.
4. Count repeated failures.
5. Correlate the failures with any subsequent successful login.
6. Review the evidence before classifying the activity.

**Threshold:** To be defined and validated during implementation.

## 5. Investigation Fields
- Timestamp
- Username
- Hostname
- Source IP, if available
- Authentication result
- Number of failures
- Related successful logins

## 6. Possible Explanations
- User entering an incorrect password
- Misconfigured service
- Brute-force activity
- Password spraying

## 7. MITRE ATT&CK
Potential reference: **T1110 — Brute Force**

Use this mapping only when the observed behaviour supports it.

## 8. Analyst Actions
- Review the underlying events.
- Check for repeated attempts against multiple accounts.
- Correlate related authentication activity.
- Escalate according to the incident response process if suspicious activity is supported by evidence.
