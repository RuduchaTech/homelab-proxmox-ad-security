# Backup Strategy

## Primary Backup Storage

QNAP NAS RAID6.

---

# Backup Targets

- VM backups,
- restore validation,
- long-term storage.

---

# Proxmox Backup Jobs

| VM | Backup |
|---|---|
| DC-01 | enabled |
| FILE-01 | enabled |
| DOCKER-01 | enabled |
| BACKUP-01 | enabled |

---

# Backup Validation

Restore testing performed using:

VM131 FILE-01-RESTORE-TEST

---
