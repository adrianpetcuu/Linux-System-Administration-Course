# System Maintenance Commands

Linux provides system maintenance commands
to safely shut down, reboot,
or change the system run state.

## shutdown
- Safely powers off or reboots the system
- Notifies logged-in users
- Examples:
  - `shutdown now` – shut down immediately
  - `shutdown -r now` – reboot immediately
  - `shutdown +5` – shut down in 5 minutes

## reboot
- Reboots the system immediately
- Equivalent to `shutdown -r now`
- Example:
  - `reboot`

## halt
- Stops all processes and halts the system
- Does not power off on all systems
- Example:
  - `halt`

## init
- Changes system runlevels (legacy systems)
- On systemd systems, replaced by `systemctl`
- Examples:
  - `init 0` – shutdown
  - `init 6` – reboot

## systemd alternatives
- `systemctl poweroff`
- `systemctl reboot`

System maintenance commands
must be used carefully
to avoid data loss
and service interruption.
