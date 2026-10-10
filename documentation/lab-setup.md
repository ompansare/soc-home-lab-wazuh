# Wazuh SOC Home Lab - Lab Setup

## Objective

This lab demonstrates the setup of a basic Security Operations Center (SOC) environment using Wazuh SIEM.

The goal is to collect security logs, monitor events, detect suspicious activity, and investigate security alerts.

## Tools Used

- Wazuh SIEM
- Linux
- Windows
- VMware
- Kali Linux
- Sysmon
- MITRE ATT&CK

## Lab Architecture

The lab consists of:

1. Wazuh Server
2. Windows Endpoint
3. Linux/Kali Linux machine
4. Security monitoring through Wazuh Dashboard

## Security Monitoring Tasks

The following activities are performed in this lab:

- Windows security event monitoring
- Failed login detection
- Successful login monitoring
- Suspicious process detection
- Authentication log analysis
- Security alert investigation
- MITRE ATT&CK technique mapping

## Investigation Workflow

When an alert is generated:

1. Review the alert severity.
2. Identify the affected endpoint.
3. Examine the timestamp.
4. Analyse the source IP address.
5. Review the related event/log.
6. Determine whether the activity is suspicious.
7. Map the activity to MITRE ATT&CK when applicable.
8. Document the investigation and conclusion.

## Learning Outcomes

Through this lab, I developed practical knowledge of:

- SIEM monitoring
- Log analysis
- Security alert investigation
- Windows/Linux security logs
- Incident detection
- Basic SOC analyst workflow
- MITRE ATT&CK framework

