# 🛡️ OSI 1–7 Defense-in-Depth Security Blueprint

## Security-Aware Systems Design for Data & Analytics Workflows

### Objective

This repository documents a defense-in-depth security baseline for a single-user workstation and home network, using the OSI model (Layers 1–7) as a control-mapping framework.

The goal is not enterprise-scale security, but a practical, auditable, and layered security posture suitable for:

-  Data professionals handling sensitive datasets

-  Analytics work in regulated environments (healthcare, finance, compliance)

-  Individuals seeking to understand security as a system, not a toolset

### Why Defense-in-Depth

Security failures rarely occur because a single tool failed.
They occur because one layer was trusted too much.

### This project demonstrates how overlapping controls:

-  Reduce blast radius

-  Limit lateral movement

-  Improve detection and recovery

-  Enforce least privilege across hardware, network, application, and user layers

### Threat Model (High-Level)

This section answers: “What are we defending against?”
Everything below exists because of these threats.

### In Scope

-  Credential compromise (phishing, password reuse)

-  Malware execution and persistence

-  Accidental or malicious data leakage

-  Network interception on untrusted Wi-Fi

-  Device loss or theft

-  Unauthorized access to sensitive analytics data

### Out of Scope

-  Enterprise SOC operations

-  Advanced nation-state threats

-  Zero-day exploitation

-  Large multi-user infrastructure

### 📄 Detailed assumptions and tradeoffs are documented in
-  /docs/00_scope_threat_model.md

### OSI Control Mapping Overview

Controls are implemented and validated at each OSI layer, ensuring no single failure compromises the system.

-  OSI Layer	Focus Area	Example Controls
-  Pre-OSI	Firmware Trust	UEFI / BIOS security, CPU microcode
-  Layer 1	Physical	TPM, Secure Boot
-  Layer 2	Data Link	Encrypted overlay networking
-  Layers 3–4	Network & Transport	Firewall, VPN encryption
-  Layer 5	Session	Encrypted sessions, secure DNS
-  Layer 6	Presentation	Disk & email encryption
-  Layer 7	Application	DLP, malware detection, secure email

### 📁 Full control documentation lives in /controls/.

### Control Documentation Structure

### Each OSI layer is documented using a consistent, auditable format:

-  isk Addressed

-  Controls Implemented

-  Implementation Summary

-  Validation Approach

-  Evidence (where applicable)

This ensures the project can be reviewed, extended, or audited without relying on tribal knowledge.

### Validation & Evidence

Where applicable, controls are validated using:

-  System configuration screenshots

-  Command outputs

-  Tool status indicators

Evidence artifacts are stored in:

-  /evidence/
    └── screenshots/


This repo emphasizes verifiable security, not just configuration claims.

### Audience

This project is designed for:

-  Data analysts and engineers in regulated domains

-  Security-aware analytics professionals

-  Junior security engineers building foundational intuition

-  Hiring managers evaluating applied security literacy
