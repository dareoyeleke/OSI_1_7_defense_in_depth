# OSI_1_7_defense_in_depth
Defense in Depth – OSI Layer Security Implementation

Tools & Technologies: BitLocker, Command Prompt, Tailscale, Windows Defender, FlowCrypt, Thunderbird, Atcalis S/MIME, Google Cloud DLP, Python, PowerShell

Project Type: Cybersecurity Configuration & System Hardening

Description:
Designed and implemented a multi-layered Defense in Depth security architecture mapped to OSI Layers 1–7, incorporating encryption, endpoint protection, and data loss prevention to safeguard system and data integrity.

Key Achievements:

Full Disk Encryption (Layers 1, 6 & 7):
Configured BitLocker via Command Prompt with TPM + PIN authentication and firmware-level security. Implemented high-complexity passwords for external drives, with recovery keys securely stored in offline environments.

Network Security with Tailscale (Layer 3):
Established encrypted connections across phone, tablet, and desktop using desktop as an exit node. Configured DNS filtering (Quad9 & Cloudflare), MagicDNS, HTTPS certificates, key expiry, and LAN isolation to reinforce zero-trust principles.

System & Firewall Protection (Layers 3, 4 & 7):
Hardened Windows Defender Firewall to allow only encrypted traffic on public, private, and domain networks, with automated weekly full scans via Task Scheduler.

Email Encryption (Layer 6):
Implemented end-to-end encryption across Gmail, Yahoo, and Apple Mail using PGP (FlowCrypt, Thunderbird) and S/MIME (Atcalis) with RSA 4096-bit keys.
Managed secure key distribution and backup for cross-device encrypted email communication.

Data Loss Prevention (Layers 6 & 7):
Integrated Google Cloud DLP to detect and alert on PII exposure in Python scripts and SQL queries using custom REGEX and OS module scanning automation in VS Code and Jupyter Notebook.

Access Control:
Configured idle session timeouts and automatic logoff protocols with pre-termination warnings to prevent unauthorized access.

Impact:
Established a robust multi-layer cybersecurity defense system securing data at the network, application, and endpoint levels, significantly reducing risk of data exposure or unauthorized access.
