#  SOC Incident Report — Failed Login Activity

## 1. Incident Summary

- **Incident Type:** Repeated Failed Login Attempts
- **Severity:** Undetermined — requires event review
- **Affected Host:** `TEST-WINDOWS-PC`
- **Source IP:** `192.0.2.25` (documentation-only example IP)
- **Status:** Simulated / Not Verified

## 2. Objective

Demonstrate how a SOC analyst could review repeated authentication failures and decide whether further investigation is needed.

## 3. Evidence Required

Before making a real finding, collect:

- Relevant Windows Security event logs
- Event timestamps and timezone
- Account names involved
- Source IP address, if recorded
- Wazuh alert details and rule ID
- Related successful or failed login events

## 4. Investigation Procedure

1. Review the alert details in Wazuh.
2. Identify the endpoint and account involved.
3. Check the timestamps and frequency of failed attempts.
4. Correlate relevant authentication events.
5. Look for successful logins following repeated failures.
6. Determine whether the activity has a legitimate explanation.
7. Document evidence, limitations, and recommended actions.

## 5. Findings

No actual findings are available because this is a simulated report and no live logs have been analysed.

## 6. Recommended Actions

If suspicious activity is confirmed during authorised testing:

- Validate the affected account with the system owner.
- Review related authentication events.
- Follow the organisation's incident response process.
- Preserve relevant logs.
- Escalate according to the confirmed risk and evidence.

## 7. Conclusion

This sample demonstrates the structure of a failed-login investigation report. The scenario has not been tested in Wazuh, and no real incident or detection capability is claimed.

## 8. MITRE ATT&CK

**Potential mapping:** T1110 — Brute Force, only if the collected evidence supports that behaviour.

## 9. Evidence Status

- [ ] Wazuh alert screenshot captured
- [ ] Relevant event logs reviewed
- [ ] Alert rule and severity verified
- [ ] Investigation completed in a test lab
- [ ] Report updated with actual evidence
