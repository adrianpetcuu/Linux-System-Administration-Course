## System Backup using dd Command

The `dd` command is a low-level
utility used to copy raw data.
It is commonly used for disk
backups, cloning, and recovery.

---

### What dd Does
- Copies data block by block
- Works with disks, partitions, and files
- Very powerful and dangerous if misused

---

### Backup a Disk
```bash
dd if=/dev/sda of=/backup/sda.img bs=4M status=progress
```

- `if` – input file (source)
- `of` – output file (destination)
- `bs` – block size

---

### Backup a Partition
```bash
dd if=/dev/sda1 of=/backup/sda1.img bs=4M status=progress
```

---

### Restore from Backup
```bash
dd if=/backup/sda.img of=/dev/sda bs=4M status=progress
```

⚠️ Warning:
- Restoring overwrites all data
- Double-check source and destination

---

### Common Use Cases
- Full disk backup
- Disk cloning
- Bootloader recovery
- Forensics

---

### Summary
`dd` creates exact disk copies
at block level and is useful
for backups and recovery,
but must be used carefully.
