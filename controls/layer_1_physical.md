# 🔌 Layer 1 – Physical

## Focus
Hardware root-of-trust and device integrity.

## Controls Implemented

### Trusted Platform Module (TPM)
- Hardware-backed key storage
- Secure cryptographic operations

### Secure Boot
- Boot chain integrity verification
- Prevents unauthorized firmware or OS loaders

- TPM-backed key storage used for BitLocker volume protection  
  (see `evidence/screenshots/tpm-protector-status.png`)


## Risks Addressed
- Device theft
- Boot-level tampering
- Offline attacks against storage

## Outcome
Establishes trust at the hardware level before OS execution.
