## Add Disk and Create New LVM Partition (pvcreate, vgcreate, lvcreate)

This guide explains how to add a new disk
and create an LVM-based partition
using Physical Volumes, Volume Groups,
and Logical Volumes.

---

### 1. Detect New Disk
After adding the disk:
```bash
lsblk
fdisk -l
```

Example new disk:
- `/dev/sdc`

---

### 2. Create Physical Volume (PV)
```bash
pvcreate /dev/sdc
```

Verify:
```bash
pvs
```

---

### 3. Create Volume Group (VG)
```bash
vgcreate vg_data /dev/sdc
```

Verify:
```bash
vgs
```

---

### 4. Create Logical Volume (LV)
```bash
lvcreate -n lv_data -L 10G vg_data
```

Verify:
```bash
lvs
```

---

### 5. Create Filesystem
```bash
mkfs.ext4 /dev/vg_data/lv_data
```

---

### 6. Mount Logical Volume
```bash
mkdir /data
mount /dev/vg_data/lv_data /data
```

Verify:
```bash
df -h
```

---

### 7. Persistent Mount
Edit `/etc/fstab`:
```text
/dev/vg_data/lv_data   /data   ext4   defaults   0 0
```

---

### Summary
Adding a disk with LVM involves
creating a Physical Volume,
adding it to a Volume Group,
creating a Logical Volume,
and mounting it for use.
