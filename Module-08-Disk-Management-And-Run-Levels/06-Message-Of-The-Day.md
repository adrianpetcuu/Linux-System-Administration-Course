## Message of the Day (MOTD)

Message of the Day (MOTD)
is a text message displayed
to users after successful login.

### Purpose
- Display system information
- Show warnings or notices
- Provide usage or policy messages

### MOTD File Location
- Static MOTD file:
  - `/etc/motd`

### Edit MOTD
```bash
vi /etc/motd
```

Example content:
```text
Welcome to the Linux Server
Unauthorized access is prohibited.
```

### Dynamic MOTD (systemd-based)
- Generated from scripts in:
  - `/etc/motd.d/`
  - `/run/motd.d/`

### Disable Dynamic MOTD (Optional)
```bash
chmod -x /etc/update-motd.d/*
```

### Summary
MOTD is used to display
important messages to users
upon login and is commonly
used in enterprise systems.
