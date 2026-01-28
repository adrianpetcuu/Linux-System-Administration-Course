## Configure and Secure SSH

SSH can be configured and secured
to protect remote access
to a Linux system.

### SSH Configuration File
- Main config file:
  - `/etc/ssh/sshd_config`

### Common Security Settings
- Disable root login
```
PermitRootLogin no
```

- Change default port (optional)
```
Port 2222
```

- Allow only specific users
```
AllowUsers user1 user2
```

### Restart SSH Service
```bash
systemctl restart sshd
```

### Firewall Configuration
Allow SSH through firewall:
```bash
firewall-cmd --add-service=ssh --permanent
firewall-cmd --reload
```

### SSH Key Authentication
- More secure than passwords
- Uses public/private key pairs

### Summary
Securing SSH involves
restricting access,
hardening configuration,
and using encryption
and key-based authentication.
