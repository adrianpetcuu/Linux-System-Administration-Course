## The xfs_info Command

The `xfs_info` command is used
to display detailed information
about an XFS filesystem.

---

### Purpose
- Show filesystem geometry
- Display block size and inode info
- Useful for troubleshooting and resizing

---

### Basic Usage
```bash
xfs_info /mount_point
```

Example:
```bash
xfs_info /data
```

---

### Information Displayed
- Filesystem name
- Block size
- Allocation groups
- Inode size
- Sector size

---

### Important Notes
- Works only on **mounted XFS filesystems**
- Does not modify data
- Read-only informational command

---

### Common Use Case
- Verify filesystem details before
  resizing with `xfs_growfs`

---

### Summary
`xfs_info` provides detailed
insight into XFS filesystem
structure and is essential
for XFS administration.
