# systemctl Command

The `systemctl` command is used
to manage services and system states
on Linux systems that use systemd.

## Common service actions
- `systemctl start service` – start a service
- `systemctl stop service` – stop a service
- `systemctl restart service` – restart a service
- `systemctl reload service` – reload configuration
- `systemctl status service` – check service status

## Enable and disable services
- `systemctl enable service` – start service at boot
- `systemctl disable service` – prevent service from starting at boot

## System control
- `systemctl reboot` – reboot the system
- `systemctl poweroff` – shut down the system

## Examples
- `systemctl status sshd`
- `systemctl enable --now firewalld`

The `systemctl` command
is essential for managing services
and troubleshooting system behavior.
