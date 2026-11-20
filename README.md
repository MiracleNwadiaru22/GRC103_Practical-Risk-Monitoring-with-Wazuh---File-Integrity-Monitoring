# Practical Risk Monitoring with Wazuh

## Overview
This project demonstrates the implementation of SIEM and File Integrity Monitoring (FIM) using **Wazuh v4.12.0** to detect changes to sensitive files and support Governance, Risk, and Compliance (GRC).

## Tools Used
- Wazuh v4.12.0
- Ubuntu Server
- Windows 11
- Kali Linux
- Wazuh Dashboard

## Implementation
- Deployed Wazuh Manager on Ubuntu Server.
- Installed and registered the Windows Wazuh Agent.
- Configured FIM to monitor `C:\Users\HOME\SensitiveFiles`.
- Verified the Windows agent was Active.

## FIM Testing
Created `Financial_Forecast.txt` and performed three tests:

| Activity | Detection |
|---|---|
| File creation | `added` |
| File modification | `modified` |
| File deletion | `deleted` |

All three events were successfully detected and reviewed through the Wazuh Dashboard using the `syscheck` filter.

## Key Outcomes
- Successfully configured real-time file monitoring.
- Detected file creation, modification, and deletion.
- Demonstrated how centralized monitoring supports security, risk management, and compliance.
