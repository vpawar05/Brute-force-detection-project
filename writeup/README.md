# SSH Brute Force Attack & Detection Lab

This project simulates an SSH brute force attack using **Hydra**, and demonstrates how to detect it using log analysis. It was built as part of a cybersecurity research project and conducted on the [TryHackMe](https://tryhackme.com/room/bruteit) platform.

## Objective

- Perform an SSH brute-force attack in a realistic lab
- Extract and analyze relevant logs (e.g., failed login attempts)
- Show how such activity could be detected by a SIEM (like ELK or Wazuh)
- Document attack mapping using the MITRE ATT&CK framework

## Tools Used

- TryHackMe Lab (Brute It)
- Hydra (attack tool)
- Linux logging (`/var/log/auth.log`)
- (Optional) Wazuh or Splunk for log ingestion and alerting
- Visuals: draw.io or Lucidchart

## Attack Summary

- Target: SSH service
- Method: Dictionary brute-force using Hydra
- Credentials used: Custom or provided wordlist
- Outcome: Successful login + detection artifacts

## Detection Summary

- Indicator: Repeated failed SSH login attempts from same IP
- Logs: Extracted from victim VM
- Example detection rule included [here](./detection/detection-rule.md)

## Screenshots

| Attack | Detection | Dashboard |
|--------|-----------|-----------|
| ![](./writeup/screenshots/brute-attack.png) | ![](./writeup/screenshots/detection-logs.png) | ![](./writeup/screenshots/dashboard.png) |

## Related

- [MITRE ATT&CK T1110 – Brute Force](https://attack.mitre.org/techniques/T1110/)
- [TryHackMe – Brute It Room](https://tryhackme.com/room/bruteit)
