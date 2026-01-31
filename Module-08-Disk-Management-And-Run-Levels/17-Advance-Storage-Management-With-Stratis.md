## Advanced Storage Management with Stratis

Stratis is a modern
storage management solution
that simplifies advanced
filesystem features on Linux.

---

### What is Stratis
- Volume-managing filesystem
- Built on top of LVM and XFS
- Provides pooling, snapshots, and monitoring
- Easier alternative to manual LVM management

---

### Key Components
- **Pool** – Collection of block devices
- **Filesystem** – Created from pool space

---

### Install Stratis
```bash
dnf install stratisd stratis-cli -y
```

### Start and Enable Service
```bash
systemctl enable --now stratisd
```

---

### Create Stratis Pool
```bash
stratis pool create pool1 /dev/sdb
```

Verify:
```bash
stratis pool list
```

---

### Create Filesystem
```bash
stratis filesystem create pool1 fs1
```

---

### Mount Filesystem
```bash
mkdir /stratis
mount /stratis/pool1/fs1 /stratis
```

---

### Persistent Mount
```bash
stratis filesystem list
```
Use UUID in `/etc/fstab`.

---

### Summary
Stratis provides simplified
advanced storage management
with pooling and snapshots
while leveraging LVM and XFS
under the hood.
