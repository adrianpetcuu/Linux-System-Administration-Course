## File System Check (fsck and xfs_repair)

Filesystem check tools are used
to detect and repair filesystem
errors caused by crashes,
power failures, or disk issues.

---

## fsck (File System Check)

`fsck` is used for
**ext2/ext3/ext4** filesystems.

### Basic Usage
```bash
fsck /dev/sdb1
```

Automatic repair:
```bash
fsck -y /dev/sdb1
```

⚠️ Best practice:
- Run fsck on **unmounted** filesystems
- Or in **rescue mode**

---

## xfs_repair

`xfs_repair` is used
**only for XFS filesystems**.

### Basic Usage
```bash
xfs_repair /dev/vg_data/lv_data
```

Repair root filesystem (rescue mode):
```bash
xfs_repair -L /dev/mapper/rhel-root
```

⚠️ Notes:
- XFS does NOT use fsck
- Filesystem must be unmounted
- `-L` may cause data loss (last resort)

---

## When to Use Which

| Filesystem | Tool |
|----------|------|
| ext4 | fsck |
| xfs | xfs_repair |

---

## Summary
- `fsck` repairs ext filesystems
- `xfs_repair` repairs XFS
- Always unmount before repair
- Critical skill for Linux admins
