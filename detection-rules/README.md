# Wazuh Detection Rules

## Overview

This section documents security detections for a Wazuh SIEM-based SOC environment.

## Detection 1: Failed Authentication

### Objective

Detect repeated failed authentication attempts on a monitored endpoint.

### Investigation Fields

The analyst should review:

- Username
- Source IP address
- Destination host
- Timestamp
- Number of failed attempts
- Authentication method
- Related security events

### Possible Security Concerns

Repeated failed authentication attempts may indicate:

- User error
- Brute-force activity
- Password spraying
- Unauthorized access attempts

### MITRE ATT&CK

Potential technique:

**T1110 – Brute Force**

The technique should only be mapped when the available evidence supports brute-force behaviour.

---

## Detection 2: Successful Login After Failed Attempts

### Objective

Identify a successful authentication occurring after multiple failed attempts.

### Investigation

Correlate:

1. Failed authentication events
2. Successful authentication
3. Source IP address
4. Username
5. Time between events

This correlation can help determine whether an account may have been compromised.

---

## Detection 3: Suspicious Authentication Activity

### Objective

Identify unusual authentication behaviour that differs from normal activity.

### Investigation Questions

- Is the source IP expected?
- Is the username legitimate?
- Did the activity occur outside normal usage?
- Were multiple accounts targeted?
- Was there a successful login afterward?

## Analyst Response

If malicious activity is confirmed:

1. Validate the affected account.
2. Review related events.
3. Investigate the source.
4. Check for additional affected accounts.
5. Reset credentials if required.
6. Contain the activity according to the incident response procedure.
7. Document the evidence.
