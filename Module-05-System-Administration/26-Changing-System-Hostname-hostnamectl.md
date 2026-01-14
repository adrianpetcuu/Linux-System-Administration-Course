# Changing System Hostname (hostnamectl)

Linux systems using systemd
allow hostname management
through the `hostnamectl` command.

## What is a hostname
- A hostname identifies a system on a network
- Used by services, logs, and network tools

## View current hostname
- `hostnamectl`
- `hostname`

## Change system hostname
- `hostnamectl set-hostname NEW_HOSTNAME`

## Example
- Set hostname to MyLinuxVM:
- `hostnamectl set-hostname MyLinuxVM`

## Apply changes
- The hostname change is immediate
- A reboot is not required
- Verify with:
- `hostnamectl`

## Notes
- Hostname is stored in `/etc/hostname`
- Root privileges are required

Changing the hostname
is a common system administration task
and is tested in RHCSA.
