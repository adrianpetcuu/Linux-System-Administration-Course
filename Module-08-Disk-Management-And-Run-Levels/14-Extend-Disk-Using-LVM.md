## Extend Disk Using LVM

This guide explains how
to extend disk space using
Logical Volume Management (LVM)
without downtime.

---

### Scenario
- Existing Logical Volume is full
- A new disk or free space is available
- Goal: extend filesystem size

---

### 1. Add New Disk or Partition
Verify new disk:
```bash
lsblk
```

Example:
- New disk: `/dev/sdd`

---

### 2. Create Physical Volume
```bash
pvcreate /dev/sdd
```

Verify:
```bash
pvs
```

---

### 3. Extend Volume Group
```bash
vgextend vg_data /dev/sdd
```

Verify:
```bash
vgs
```

---

### 4. Extend Logical Volume
Extend by size:
```bash
lvextend -L +5G /dev/vg_data/lv_data
```

Or use all free space:
```bash
lvextend -l +100%FREE /dev/vg_data/lv_data
```

---

### 5. Resize Filesystem

For **ext4**:
```bash
resize2fs /dev/vg_data/lv_data
```

For **xfs**:
```bash
xfs_growfs /data
```

---

### 6. Verify
```bash
df -h
```

---

### Summary
LVM allows disks and filesystems
to be extended online by
adding storage, extending
volume groups, and resizing
the filesystem safely.
