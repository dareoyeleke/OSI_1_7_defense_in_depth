# 🧠 Layer 7 – Application

## Focus
Application-level data protection, malware prevention, and user-facing security controls.

## Controls Implemented

### Google Cloud DLP
- Regex-based content inspection using `re` and `os` modules
- Detection of sensitive data patterns (PII) in files and scripts
- Used as a lightweight Data Loss Prevention (DLP) mechanism

### Microsoft Defender
- Real-time malware detection
- Scheduled scans and signature updates
- Application-level threat prevention
- 
### Secure Email Applications
- Secure email workflows implemented using FlowCrypt (webmail) and Thunderbird
- Application-level controls enforce encrypted content handling and signing
- Cryptographic enforcement is handled at the Presentation layer
(See Layer 6 for encryption and key management details)

## Risks Addressed
- Malware execution
- Accidental or malicious data leakage
- Phishing and unsafe email content

## Outcome
Provides first-line defense where users directly interact with data and applications.
