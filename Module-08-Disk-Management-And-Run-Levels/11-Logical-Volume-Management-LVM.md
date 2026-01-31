## Logical Volume Management (LVM)

LVM allows flexible
disk management by
abstracting physical
storage into logical volumes.

### LVM Components
- **Physical Volume (PV)** – Disk or partition
- **Volume Group (VG)** – Pool of storage
- **Logical Volume (LV)** – Usable storage unit

---

### 1. Create Physical Volume
```bash
pvcreate /dev/sdb1
```

### 2. Create Volume Group
```bash
vgcreate vg_data /dev/sdb1
```

### 3. Create Logical Volume
```bash
lvcreate -n lv_data -L 5G vg_data
```

---

### 4. Create Filesystem
```bash
mkfs.ext4 /dev/vg_data/lv_data
```

---

### 5. Mount Logical Volume
```bash
mkdir /data
mount /dev/vg_data/lv_data /data
```

---

### 6. Persistent Mount
Edit `/etc/fstab`:
```text
/dev/vg_data/lv_data   /data   ext4   defaults   0 0
```

---

### Useful LVM Commands
```bash
pvs
vgs
lvs
```

---

### Summary
LVM provides flexible
storage management with
easy resizing, snapshots,
and better disk utilization.
