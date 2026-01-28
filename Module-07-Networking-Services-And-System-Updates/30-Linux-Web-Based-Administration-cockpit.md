## Linux Web Based Administration (Cockpit)

Cockpit is a web-based
administration interface
for managing Linux servers.

### Key Features
- Web-based system management
- Monitor system resources
- Manage services, users, and storage
- Integrated with systemd

### Install Cockpit
```bash
dnf install cockpit -y
```

### Start and Enable Cockpit Socket
```bash
systemctl enable --now cockpit.socket
```

### Access Cockpit
Open in browser:
```
https://server_ip:9090
```

### Firewall Configuration
```bash
firewall-cmd --add-service=cockpit --permanent
firewall-cmd --reload
```

### Authentication
- Login with a regular user
- User must have sudo privileges
- Root login is disabled by default

### Summary
Cockpit provides an easy
and secure way to manage
Linux servers through
a web browser.
