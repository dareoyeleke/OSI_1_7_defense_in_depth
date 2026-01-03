# 🌐 Layer 5 – Session

## Focus
Secure session establishment, persistence, and encryption.

## Controls Implemented

### Tailscale (WireGuard VPN)
- Encrypted device-to-device sessions
- Identity-based networking

### Encrypted DNS
- DNS over HTTPS (DoH)
- DNS over TLS (DoT)
- Prevents DNS interception and profiling\

## Evidence

- Encrypted device-to-device sessions established using Tailscale (WireGuard VPN), 
  with a validated active exit node routing traffic securely  
  (see `evidence/screenshots/tailscale-active-exit-node.png`)

- Encrypted DNS resolution and threat filtering enforced via Quad9 DNS, 
  confirmed at the client/browser level  
  (see `evidence/screenshots/quad9-dns-filtering-browser.png`)


## Risks Addressed
- Session hijacking
- DNS spoofing
- Traffic inspection on untrusted networks

## Outcome
Maintains session confidentiality and integrity across networks.
