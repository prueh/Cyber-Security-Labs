# Week 2: SOC Operations & SIEM Foundations
## Objective
To transition the security environment from basic setup to a functional Security Operations Center (SOC) posture using **Wazuh SIEM**.

## Key Achievements
* **File Integrity Monitoring (FIM):** Configured the `syscheck` module in `ossec.conf` for real-time monitoring of critical system files in `/etc`.
* **Rule Engineering:** Developed custom XML detection rules to identify unauthorized administrative changes and SSH configuration tampering.
* **Active Response:** Implemented an automated "Firewall-Drop" script. Configured the Wazuh Manager to command the Linux agent to update `iptables` and block source IPs after 6 failed SSH attempts.
* **Windows Event Analysis:** Analyzed Event IDs 4625 (Failed Login) and 4720 (User Provisioning) to distinguish between brute force attacks and legitimate administrative actions.

## Tools Used
* **Wazuh SIEM** (Manager & Agents)
* **Linux (Ubuntu)** & **Windows 10**
* **iptables** for Active Response
