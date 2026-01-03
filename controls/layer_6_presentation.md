# 🔐 Layer 6 – Presentation

## Focus
Data confidentiality, integrity, and cryptographic protection.

## Controls Implemented

### BitLocker
- Full disk encryption for data-at-rest
- TPM-backed key storage

### FlowCrypt (PGP)
- End-to-end email encryption
- Protects message content in transit and at rest

### S/MIME
- Certificate-based email encryption
- Digital signing for message authenticity

## Evidence

- Full disk encryption enabled on system volume using BitLocker  
  (see `evidence/screenshots/bitlocker-system-drive-status.png`)

- External storage encrypted using BitLocker to protect removable media  
  (see `evidence/screenshots/bitlocker-external-drive-status.png`)

- Encryption keys protected using hardware-backed TPM  
  (see `evidence/screenshots/tpm-protector-status.png`)

- PGP key pair configured and active for end-to-end email encryption and signing  
  (see `evidence/screenshots/flowcrypt-pgp-key-configured.png` and 'evidence/screenshots/thunderbird-pgp-key-configured.png')



## Risks Addressed
- Unauthorized access to stored data
- Email interception or tampering
- Loss of confidentiality during data exchange

## Outcome
Ensures data remains protected regardless of transport or storage medium.
