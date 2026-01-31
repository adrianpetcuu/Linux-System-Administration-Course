## Storage in Linux

Linux storage refers to how
disks, partitions, and filesystems
are organized and managed.

### Storage Devices
- Physical disks: `/dev/sda`, `/dev/sdb`
- Virtual disks in VMs
- Block devices

### Partitions
- Divide disks into sections
- Common tools:
```bash
lsblk
fdisk
parted
```

### Filesystems
- Format partitions for data storage
- Common filesystems:
  - ext4
  - xfs
  - vfat

Create filesystem:
```bash
mkfs.ext4 /dev/sdb1
```

### Mounting
- Attach filesystem to directory

```bash
mount /dev/sdb1 /data
```

Mount points:
- `/`
- `/home`
- `/var`
- `/data`

### Persistent Mounts
- Configured in `/etc/fstab`

### Summary
Linux storage includes
disks, partitions, filesystems,
and mount points and is
essential for system operation.
