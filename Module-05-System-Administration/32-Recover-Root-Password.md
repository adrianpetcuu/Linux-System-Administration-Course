# Recover Root Password

Linux allows recovery of the root password
using the bootloader and single-user mode.

## When is this needed
- Root password is forgotten
- No sudo access is available
- Physical or console access exists

## Recovery method (systemd systems)
1. Reboot the system
2. At the GRUB menu, select the kernel and press `e`
3. Find the line starting with `linux` or `linux16`
4. Add at the end of the line:
```
rd.break
```
5. Press `Ctrl + X` to boot

## Reset the password
- Remount filesystem as read-write:
```
mount -o remount,rw /sysroot
chroot /sysroot
```
- Set new root password:
```
passwd
```
- Relabel SELinux:
```
touch /.autorelabel
```
- Exit and reboot:
```
exit
reboot
```

Root password recovery
is a standard administrative task
and commonly tested in RHCSA.
