```markdown
# VLAN Plan

| VLAN | Name | Subnet | Gateway |
|---|---|---|---|
| 10 | DOM | 192.168.10.0/24 | ER605 |
| 20 | LAB | 192.168.20.0/24 | OPNsense |

---

# Switch Port Allocation

| Port | Device | VLAN |
|---|---|---|
| 1 | QNAP LAN1 | 10 |
| 3 | QNAP LAN2 | 20 |
| 5 | Workstation R9 | 10 |
| 7 | Dell 5820 | Trunk |
| 9 | ThinkPad L14 | 10 |
| 11 | Workstation R7 | 10 |
| 15 | WAN / ISP | WAN |
---

# Design Notes

- QNAP uses dual connectivity.
- Dell Proxmox node receives VLAN-aware trunk.
- LAB environment isolated from home traffic.
- Static VLAN configuration remains active permanently.
