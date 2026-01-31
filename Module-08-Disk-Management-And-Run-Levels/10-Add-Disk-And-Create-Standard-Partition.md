## Add Disk and Create Standard Partition

This process describes how
to add a new disk and create
a standard partition in Linux.

### 1. Detect New Disk
After adding a disk to the system:
```bash
lsblk
fdisk -l
```

New disk example:
- `/dev/sdb`

---

### 2. Create Partition with fdisk
```bash
fdisk /dev/sdb
```

Inside fdisk:
- `n` – create new partition
- `p` – primary partition
- Accept defaults for size
- `w` – write changes

---

### 3. Create Filesystem
Format the new partition:
```bash
mkfs.ext4 /dev/sdb1
```

---

### 4. Create Mount Point
```bash
mkdir /data
```

---

### 5. Mount the Partition
```bash
mount /dev/sdb1 /data
```

Verify:
```bash
df -h
```

---

### 6. Persistent Mount (fstab)
Edit:
```bash
vi /etc/fstab
```

Add:
```text
/dev/sdb1   /data   ext4   defaults   0 0
```

---

### Summary
Adding a disk involves
detecting the device,
partitioning it, creating
a filesystem, and mounting
it permanently.
