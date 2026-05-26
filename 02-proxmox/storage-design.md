```markdown
# Storage Design

## Local Storage

| Storage | Type | Purpose |
|---|---|---|
| local | directory | ISO and templates |
| tank-vm | LVM/ext4 | VM storage |

---

# Backup Storage

QNAP RAID6 NAS used for:

- VM backup,
- restore testing,
- long-term retention.

---

# Backup Strategy

| Backup Type | Retention |
|---|---|
| Daily | 3 copies |
| Weekly | 2 copies |
| Monthly | 1 copy |
