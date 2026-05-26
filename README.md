# HomeLab — Proxmox + Active Directory + Security

## Overview

This repository documents a complete educational and recruitment-oriented HomeLab environment built on:

- Proxmox VE
- Windows Server
- Active Directory
- OPNsense
- Docker
- Monitoring and backup services
- Hybrid-ready Microsoft identity design

The project was designed as:

- practical SysAdmin portfolio,
- cyber security learning environment,
- YouTube educational project,
- technical GitHub showcase.

---

# Infrastructure

## Hardware

| Device | Purpose |
|---|---|
| Dell Precision 5820 | Main Proxmox virtualization host |
| Xeon W-2155 + 64GB ECC | Compute platform |
| QNAP RAID6 NAS | Backup storage |
| TP-Link ER605 | Home network router |
| TP-Link TL-SG1016PE | VLAN managed switch |
| Lenovo ThinkPad L14 | Admin workstation |

---

# VLAN Design

| VLAN | Name | Purpose |
|---|---|---|
| 10 | DOM | Home devices |
| 20 | LAB | HomeLab infrastructure |

---

# VM Layout

| VM ID | Hostname | Role |
|---|---|---|
| 100 | OPNsense | Firewall / LAB Gateway |
| 110 | DC-01 | Active Directory |
| 120 | CL-01-WIN11 | Windows 11 domain client |
| 130 | FILE-01 | SMB file server |
| 131 | FILE-01-RESTORE-TEST | Backup restore validation |
| 140 | MGMT-01-LINUX | Linux administration node |
| 150 | SEC-01-SIEM-LITE | Monitoring / SOC-lite |
| 160 | DOCKER-01 | Container platform |
| 170 | BACKUP-01 | Backup validation node |
| 180 | HYBRID-01 | Hybrid-readiness server |

---

# Main Objectives

## Project 1 — On-prem Windows + Security

- Active Directory
- DNS / DHCP
- OU structure
- Group Policy
- Windows hardening
- SMB file server
- Backup and restore

## Project 2 — Hybrid-readiness

- Hybrid identity preparation
- UPN suffix design
- Service account for synchronization
- Microsoft Entra readiness
- RBAC concepts
- MFA planning

---

# Technologies

- Proxmox VE
- Windows Server 2022
- Active Directory
- OPNsense
- Docker
- Portainer
- Grafana
- Loki
- Uptime Kuma
- QNAP NAS
- SMB/CIFS
- Linux
- VLAN
- Backup and Restore

---

# Repository Goals

This repository demonstrates:

- infrastructure deployment,
- virtualization,
- identity management,
- network segmentation,
- backup strategy,
- monitoring,
- documentation standards,
- practical HomeLab engineering.

---
