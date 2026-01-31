## LVM Configuration During Installation

LVM can be configured
during Linux installation
to provide flexible and
scalable storage management
from the start.

### When LVM Is Used
- Default option in many installers
- Recommended for servers
- Allows easy disk resizing later

---

### LVM Setup During Installation
During the installer (Anaconda):

1. Select **Installation Destination**
2. Choose disk(s)
3. Select **Custom** or **Automatic with LVM**
4. Enable **LVM**
5. Installer creates:
   - Physical Volumes (PV)
   - Volume Group (VG)
   - Logical Volumes (LV)

---

### Typical LVM Layout
- `/` → Logical Volume
- `/home` → Logical Volume
- `swap` → Logical Volume

Example:
- VG: `rhel`
- LV: `root`, `home`, `swap`

---

### Advantages of LVM at Install Time
- Resize partitions easily
- Add disks without reinstall
- Better storage flexibility
- Snapshots support

---

### Verify LVM After Installation
```bash
lsblk
pvs
vgs
lvs
```

---

### Summary
Configuring LVM during
installation simplifies
storage management and
is best practice for
enterprise Linux systems.
