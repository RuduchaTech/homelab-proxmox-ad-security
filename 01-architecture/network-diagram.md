# Network Architecture

## Physical Topology

```text
ISP Technicolor Modem
        │
        ├── TP-Link ER605 (DOM network)
        │       ├── TV
        │       ├── Xbox
        │       └── WiiM
        │
        └── Dell Precision 5820 (OPNsense WAN)

Dell Precision 5820
│
├── Proxmox VE
│   ├── VM100 OPNsense
│   ├── VM110 DC-01
│   ├── VM120 CL-01-WIN11
│   ├── VM130 FILE-01
│   ├── VM140 MGMT-01-LINUX
│   ├── VM150 SEC-01-SIEM-LITE
│   ├── VM160 DOCKER-01
│   ├── VM170 BACKUP-01
│   └── VM180 HYBRID-01
│
└── TP-Link TL-SG1016PE
        ├── QNAP NAS
        ├── Workstation R9
        ├── Workstation R7
        └── ThinkPad L14

Design Principles
LAB network isolated from home network.
OPNsense acts as LAB firewall.
ER605 remains main household router.
Dell server does not need to run 24/7.
Home devices remain operational even when LAB is powered off.
VLAN segmentation implemented permanently on switch.
