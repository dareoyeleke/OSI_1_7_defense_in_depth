# 🛡️ OSI 1–7 Defense-in-Depth Security Blueprint

## Security-Aware Systems Design for Data & Analytics Workflows

### Objective

This repository documents a defense-in-depth security baseline for a single-user workstation and home network, using the OSI model (Layers 1–7) as a control-mapping framework.

The goal is not enterprise-scale security, but a practical, auditable, and layered security posture suitable for:

- Data professionals handling sensitive datasets  
- Analytics work in regulated environments (healthcare, finance, compliance)  
- Individuals seeking to understand security as a system, not a toolset  

---

## Why Defense-in-Depth

Security failures rarely occur because a single tool fails.  
They occur because one layer is trusted too much.

This project demonstrates how overlapping controls:

- Reduce blast radius  
- Limit lateral movement  
- Improve detection and recovery  
- Enforce least privilege across hardware, network, application, and user layers  

---

## Threat Model (High-Level)

This section answers a single question:

**What are we defending against, and why were these controls chosen?**

### In Scope

- Credential compromise (phishing, password reuse)
- Malware execution and persistence
- Accidental or malicious data leakage
- Network interception on untrusted Wi-Fi
- Device loss or theft
- Unauthorized access to sensitive analytics data

### Out of Scope

- Enterprise SOC operations
- Advanced nation-state threats
- Zero-day exploitation
- Large multi-user or cloud infrastructure

### Assumptions & Design Constraints

- The system is operated by a single trusted user
- Administrative access is available for system configuration
- Firmware and OS are assumed uncompromised at initial setup
- Confidentiality is prioritized over high availability
- Controls must not significantly disrupt daily analytics workflows
  
---

## OSI Control Mapping Overview

Controls are implemented across OSI layers to ensure no single failure compromises the system.

| OSI Layer | Focus Area | Example Controls |
|---------|------------|------------------|
| Pre-OSI | Firmware Trust | UEFI/BIOS security, CPU microcode |
| Layer 1 | Physical | TPM, Secure Boot |
| Layer 2 | Data Link | Encrypted overlay networking |
| Layers 3–4 | Network & Transport | Firewall rules, VPN encryption |
| Layer 5 | Session | Encrypted sessions, secure DNS |
| Layer 6 | Presentation | Disk encryption, email encryption |
| Layer 7 | Application | DLP, malware detection, secure email clients |

📁 Full control documentation lives in `/controls/`.

---

## Control Documentation Structure

Each OSI layer is documented using a consistent, auditable format:

- Risk Addressed  
- Controls Implemented  
- Implementation Summary  
- Validation Approach  
- Evidence (where applicable)  

This ensures the system can be reviewed, extended, or audited without relying on tribal knowledge.

---

## Validation & Evidence

Controls are validated using:

- System configuration screenshots  
- Command-line verification outputs  
- Tool status indicators  

Evidence artifacts are stored under:

/evidence/
└── screenshots/


Validated controls include (non-exhaustive):

- Full disk encryption for system and external drives with TPM-backed key protection
- Encrypted VPN sessions with an active exit node
- DNS-layer threat filtering via Quad9
- End-to-end email encryption using OpenPGP and S/MIME

This repository emphasizes **verifiable security**, not configuration claims.

---

## Audience

This project is designed for:

- Data analysts and engineers working in regulated domains  
- Security-aware analytics professionals  
- Junior security engineers building foundational intuition  
- Hiring managers evaluating applied security literacy 
