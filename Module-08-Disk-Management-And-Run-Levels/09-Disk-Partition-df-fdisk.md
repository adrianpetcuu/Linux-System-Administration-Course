## Disk Partitioning (df, fdisk)

Disk partitioning allows
a physical disk to be divided
into logical sections for storage.

### df Command
- Shows disk space usage
- Displays mounted filesystems

```bash
df -h
```

Common options:
- `-h` human-readable sizes
- `-T` show filesystem type

---

### fdisk Command
- Used to create and manage partitions
- Works on MBR partition tables

List disks:
```bash
fdisk -l
```

Create or modify partitions:
```bash
fdisk /dev/sdb
```

Common fdisk actions:
- `n` create new partition
- `d` delete partition
- `p` print partition table
- `w` write changes

---

### Important Notes
- fdisk modifies disk layout
- Changes take effect after writing
- Filesystem must be created after partitioning

### Summary
`df` monitors disk usage,
while `fdisk` manages disk
partitions and layout.
