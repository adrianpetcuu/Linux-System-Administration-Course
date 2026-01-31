## Adding Swap Space

Swap space is used by Linux
as virtual memory when
physical RAM is fully utilized.

---

### Check Existing Swap
```bash
swapon --show
free -h
```

---

## Method 1: Add Swap Using a File (Recommended)

### 1. Create Swap File
```bash
fallocate -l 2G /swapfile
```

### 2. Set Permissions
```bash
chmod 600 /swapfile
```

### 3. Create Swap Area
```bash
mkswap /swapfile
```

### 4. Enable Swap
```bash
swapon /swapfile
```

Verify:
```bash
swapon --show
```

---

### 5. Persistent Swap
Edit `/etc/fstab`:
```text
/swapfile none swap sw 0 0
```

---

## Method 2: Add Swap Using LVM

### 1. Create Logical Volume
```bash
lvcreate -L 2G -n lv_swap vg_data
```

### 2. Create Swap
```bash
mkswap /dev/vg_data/lv_swap
swapon /dev/vg_data/lv_swap
```

---

### Summary
Swap space helps prevent
out-of-memory errors and
can be added dynamically
using swap files or LVM
without reinstalling the OS.
