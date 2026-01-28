## Securing Linux Machine (OS Hardening)

OS hardening is the process
of securing a Linux system
by reducing vulnerabilities
and attack surfaces.

### User and Access Control
- Disable root SSH login
- Use sudo for privilege escalation
- Remove unused user accounts

```bash
passwd -l user
```

### SSH Hardening
Edit:
```text
/etc/ssh/sshd_config
```

Recommended settings:
```
PermitRootLogin no
PasswordAuthentication no
```

Restart SSH:
```bash
systemctl restart sshd
```

### Firewall Configuration
- Enable firewall
- Allow only required services

```bash
systemctl enable --now firewalld
firewall-cmd --list-all
```

### System Updates
- Keep system up to date

```bash
dnf update
```

### Disable Unused Services
```bash
systemctl list-unit-files --type=service
systemctl disable service_name
```

### File Permissions
- Apply least privilege principle
- Protect critical files

### Summary
OS hardening improves
system security by
restricting access,
reducing exposure,
and maintaining updates.
