## Customize Message of the Day (MOTD)

Customizing the Message of the Day
allows administrators to display
useful information or warnings
to users at login.

### Static MOTD Customization
Edit the MOTD file:
```bash
vi /etc/motd
```

Example:
```text
Welcome to Production Server
All actions are logged.
```

### Dynamic MOTD (systemd-based)
Dynamic MOTD is generated using scripts.

Directories:
- `/etc/motd.d/`
- `/run/motd.d/`

Each script outputs text
displayed at login.

### Create Custom Dynamic MOTD Script
```bash
vi /etc/motd.d/custom.sh
```

Example:
```bash
#!/bin/bash
echo "Hostname: $(hostname)"
echo "Date: $(date)"
```

Make executable:
```bash
chmod +x /etc/motd.d/custom.sh
```

### Disable Dynamic MOTD (Optional)
```bash
chmod -x /etc/update-motd.d/*
```

### Summary
MOTD customization improves
user awareness by displaying
system information, warnings,
or policies at login.
