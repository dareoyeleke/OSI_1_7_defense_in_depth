# 🔐 Layer 6 – Presentation

## Focus
Data confidentiality, integrity, and cryptographic protection.

## Controls Implemented

### BitLocker
- Full disk encryption for data-at-rest
- TPM-backed key storage
## Evidence

- Full disk encryption enabled on system volume using BitLocker  
  (see `evidence/bitlocker-system-drive-status.png`)

- External storage encrypted using BitLocker to protect removable media  
  (see `evidence/bitlocker-external-drive-status.png`)

- Encryption keys protected using hardware-backed TPM  
  (see `evidence/tpm-protector-status.png`)


### Email Encryption (PGP / S-MIME)

- OpenPGP encryption implemented via FlowCrypt for webmail
- Private keys protected with user-defined passphrase
- Client-side encryption ensures confidentiality and integrity prior to transport

**Evidence**
- (see 'evidence/flowcrypt-private-key-passphrase.png')
- (see 'evidence/thunderbird-encryption-settings.png')


## Risks Addressed
- Unauthorized access to stored data
- Email interception or tampering
- Loss of confidentiality during data exchange

## Outcome
Ensures data remains protected regardless of transport or storage medium.
