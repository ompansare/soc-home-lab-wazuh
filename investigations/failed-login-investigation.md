# Failed Login Investigation Report

## 1. Report Information
- **Project:** SOC Home Lab Using Wazuh SIEM
- **Investigation Type:** Failed Authentication
- **Report Type:** Sample / Simulated Investigation
- **Status:** Not Tested — No Live Logs Analysed
- **Environment:** Planned Wazuh SIEM Lab

## 2. Objective
The objective of this sample investigation is to document how a SOC analyst would review repeated failed authentication attempts and determine whether the activity may indicate unauthorized access.

## 3. Scenario
A monitored endpoint records multiple failed login attempts for a user account within a short period.

**Important:** This is a hypothetical scenario created for documentation and has not been observed in a live environment.

## 4. Evidence Required
The following evidence would be required for a real investigation:

- Event timestamps
- Username
- Source IP address, if available
- Hostname
- Authentication result
- Number and frequency of failed attempts
- Related successful login events

**Evidence collected:** None. No live logs have been analysed.

## 5. Investigation Procedure
1. Review authentication failure events.
2. Identify the affected account and host.
3. Compare timestamps and the frequency of attempts.
4. Check whether multiple accounts were targeted.
5. Review nearby successful login events.
6. Determine whether the activity is consistent with user error or potentially malicious behaviour.

## 6. Potential Risks
Repeated failed logins may be associated with:
- Incorrect passwords
- Brute-force attempts
- Password spraying
- Unauthorized access attempts

These are possibilities, not confirmed findings.

## 7. Sample Assessment
- **Confirmed malicious activity:** Not determined
- **True positive / false positive:** Not classified
- **Severity:** Not assigned
- **Reason:** No actual event logs or supporting evidence are available.

## 8. Recommended Response
If a real investigation confirms malicious activity, the SOC analyst should follow the organisation's incident response process, review affected accounts, preserve evidence, and escalate the incident when appropriate.

## 9. MITRE ATT&CK
Potential reference: **T1110 — Brute Force**

This mapping is relevant only if the actual evidence supports brute-force behaviour.

## 10. Conclusion
This report demonstrates a proposed investigation workflow for failed authentication events. It does not establish that an attack occurred, and no live Wazuh alert has been verified.


