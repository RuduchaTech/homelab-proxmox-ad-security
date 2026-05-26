```markdown
# Proxmox VE 9.1 Installation

## Host Hardware

- Dell Precision 5820
- Xeon W-2155
- 64GB ECC RAM
- Intel i350 dual NIC
- 2x NVMe SSD
- 2x SATA SSD

---

# Installation Goals

- stable HomeLab platform,
- low-noise operation,
- educational infrastructure,
- virtualization for Windows and Linux workloads.

---

# Installation Steps

1. Create bootable USB.
2. Disable Secure Boot in BIOS.
3. Boot Proxmox VE 8.4 installer.
4. Select graphical installation.
5. Configure storage layout.
6. Configure management IP.
7. Complete installation.
8. Install VirtIO drivers.
9. Enable VLAN awareness.
10. Configure update repositories.

---

# Storage Layout

## Recommended Layout

| Storage | Purpose |
|---|---|

Filesystem:

```text
ext4 + LVM

Reason:

lower RAM overhead,
simpler management,
suitable for 64GB environment.
| local | ISO / templates |
| tank-vm | VM disks |
| qnap-backup | backup storage |
