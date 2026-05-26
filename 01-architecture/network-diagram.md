# Diagram sieci

## Architektura logiczna

```text
ISP / Technicolor
│
├── ER605 (DOM)
│   ├── TV
│   ├── XBOX
│   ├── WiiM
│   └── VLAN 10
│
└── OPNsense VM100 (LAB)
    └── VLAN 20
        ├── DC-01
        ├── FILE-01
        ├── CL-01-WIN11
        ├── DOCKER-01
        ├── SEC-01
        ├── BACKUP-01
        └── HYBRID-01
Założenia architektury
separacja sieci DOM i LAB,
brak wpływu HomeLab na urządzenia domowe,
możliwość wyłączania Dell 5820 poza godzinami pracy LAB,
centralny backup do QNAP,
monitoring środowiska,
możliwość publikacji projektu jako portfolio.
