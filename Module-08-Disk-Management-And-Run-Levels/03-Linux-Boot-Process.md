# Linux Boot Process

This document explains the Linux boot process in a clear, step-by-step manner. Useful for Linux administration and RHCSA preparation.

---

## 1. BIOS / UEFI
- Performs hardware initialization (POST)
- Locates a bootable device
- Loads the bootloader from disk

---

## 2. Bootloader (GRUB2)
- Default bootloader on most Linux systems
- Loads the Linux kernel and initramfs
- Allows kernel parameters and OS selection

Files:
- /boot/grub2/grub.cfg
- /etc/default/grub

---

## 3. Linux Kernel
- Decompresses itself into memory
- Detects hardware
- Initializes drivers
- Mounts the initial RAM filesystem (initramfs)

---

## 4. initramfs
- Temporary root filesystem in RAM
- Loads required drivers
- Mounts the real root filesystem

---

## 5. systemd (PID 1)
- First userspace process
- Manages system services
- Loads target (runlevel equivalent)

Common targets:
- multi-user.target
- graphical.target
- rescue.target
- emergency.target

---

## 6. Login Prompt
- System ready for user interaction
- Console login or graphical login manager starts

---

## Boot Process Summary
BIOS/UEFI → GRUB → Kernel → initramfs → systemd → Login

---

## Useful Commands
```bash
systemctl get-default
systemctl set-default multi-user.target
journalctl -b
```

---

## RHCSA Notes
- Understand GRUB recovery
- Know how to interrupt boot and reset root password
- Be familiar with systemd targets
