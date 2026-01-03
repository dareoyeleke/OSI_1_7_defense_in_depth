# 🌐 Layers 3–4 – Network & Transport

## Focus
Secure data transport and network traffic control.

## Controls Implemented

### Windows Defender Firewall
- Inbound and outbound traffic filtering
- Rule-based network segmentation

### Tailscale (WireGuard)
- Encrypted transport-layer communication
- Secure routing over public networks

- Secure transport and routing enforced through WireGuard-based VPN overlay 
  with centralized exit node  
  (see `evidence/tailscale-active-exit-node.png`)


## Risks Addressed
- Network interception
- Unauthorized inbound connections
- Lateral movement

## Outcome
Reduces attack surface at the network and transport layers.
