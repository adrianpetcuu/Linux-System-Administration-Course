# Linux Boot Process (Newer Versions)

This document describes the modern Linux boot process
used by current distributions (RHEL, CentOS Stream, Fedora, Ubuntu)
based on **UEFI + GRUB2 + systemd**.

---

## 1. Power On & UEFI
- System firmware initializes hardware
- Performs POST
- Loads EFI bootloader from EFI System Partition (ESP)

Location:
- `/boot/efi/EFI/`

---

## 2. GRUB2 Bootloader
- Loads kernel and initramfs
- Allows kernel parameters and boot options

Key files:
- `/boot/grub2/grub.cfg`
- `/etc/default/grub`

---

## 3. Linux Kernel
- Decompresses into memory
- Detects hardware
- Initializes drivers
- Mounts initramfs

Kernel file:
- `/boot/vmlinuz-*`

---

## 4. initramfs
- Temporary root filesystem in RAM
- Loads required drivers (disk, LVM, RAID)
- Mounts real root filesystem

File:
- `/boot/initramfs-*.img`

---

## 5. systemd (PID 1)
- First userspace process
- Replaces SysV init
- Starts system services in parallel
- Uses targets instead of runlevels

Common targets:
- `multi-user.target`
- `graphical.target`
- `rescue.target`
- `emergency.target`

---

## 6. Login Services
- Console login (getty)
- Graphical login manager (GDM, SDDM)

---

## Boot Flow Summary
UEFI → GRUB2 → Kernel → initramfs → systemd → Login

---

## Useful Commands
```bash
systemctl get-default
systemctl set-default graphical.target
journalctl -b
```

---

## Key Differences vs Older Systems
- UEFI replaces BIOS
- systemd replaces SysV init
- Targets replace runlevels
- Faster parallel boot process
