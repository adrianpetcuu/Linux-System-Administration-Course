
# Computer Boot Process (Linux)

## Overview
The boot process is the sequence of steps a computer follows to load the operating system.

## Boot Process Steps
1. **Power On**
   - Hardware is powered on
2. **BIOS / UEFI**
   - Performs POST (Power-On Self Test)
   - Finds boot device
3. **MBR / GPT**
   - Loads bootloader
4. **GRUB**
   - Displays boot menu
   - Loads Linux kernel and initramfs
5. **Kernel**
   - Initializes hardware
   - Mounts root filesystem
6. **systemd**
   - Starts system services
   - Reaches default target

## Key Files
- `/boot/vmlinuz-*` – Linux kernel
- `/boot/initramfs-*` – Initial RAM disk
- `/etc/default/grub` – GRUB configuration

## Important Commands
- `systemctl get-default`
- `systemctl set-default multi-user.target`
- `reboot`
- `shutdown -h now`

## Summary
Understanding the boot process helps troubleshoot startup issues and is critical for system administration and RHCSA exams.
