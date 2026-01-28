## System Upgrade and Patch Management

System upgrade and patch management
ensure that a Linux system remains
secure, stable, and up to date.

### System Updates
- Apply security fixes and bug patches
- Update installed packages from repositories

```bash
dnf update
dnf upgrade
```

### System Upgrade
- Upgrades the system to newer package versions
- May update kernel and core components
- Usually requires a reboot

```bash
dnf upgrade --refresh
reboot
```

### Patch Management
- Regularly applying security patches
- Reduces vulnerabilities and exploits
- Common practice in production environments

### Best Practices
- Test updates in non-production systems
- Take backups before major upgrades
- Schedule updates during maintenance windows
- Monitor system after updates

### Check Update History
```bash
dnf history
```

### Summary
System upgrades and patch management
are critical administrative tasks
that maintain system security,
reliability, and performance.
