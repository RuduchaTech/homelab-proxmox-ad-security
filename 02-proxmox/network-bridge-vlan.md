# Proxmox Network Bridges and VLANs

## vmbr0

Main VLAN-aware bridge.

### VLANs

| VLAN | Purpose |
|---|---|
| 10 | DOM |
| 20 | LAB |

---

# Design

- Dell server connected through trunk port.
- OPNsense handles LAB routing.
- Home network isolated from LAB infrastructure.
- VLAN awareness enabled in Proxmox bridge.
