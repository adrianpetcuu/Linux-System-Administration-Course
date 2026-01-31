## Difference Between CentOS / Red Hat 5, 6, and 7

CentOS and Red Hat Enterprise Linux (RHEL)
have evolved significantly across versions,
especially in system management and boot processes.

---

## CentOS / RHEL 5
- Released around 2007
- Uses **SysV init**
- Service management with `service` and `chkconfig`
- Legacy hardware support
- EXT3 filesystem by default

Example commands:
```bash
service httpd start
chkconfig httpd on
```

---

## CentOS / RHEL 6
- Released around 2010
- Hybrid system:
  - SysV init + Upstart
- Faster boot than version 5
- EXT4 filesystem supported
- Partial modernization

Example commands:
```bash
service httpd restart
chkconfig httpd on
```

---

## CentOS / RHEL 7
- Released around 2014
- Uses **systemd**
- New service management (`systemctl`)
- Parallel service startup
- XFS filesystem by default
- Improved performance and scalability

Example commands:
```bash
systemctl start httpd
systemctl enable httpd
```

---

## Key Differences Summary

| Feature | RHEL/CentOS 5 | RHEL/CentOS 6 | RHEL/CentOS 7 |
|------|------|------|------|
| Init system | SysV | SysV + Upstart | systemd |
| Service mgmt | service | service | systemctl |
| Filesystem | ext3 | ext4 | xfs |
| Boot speed | Slow | Medium | Fast |
| Modern support | Low | Medium | High |

---

## Summary
Each version introduced
major improvements in boot,
service management, and
performance, with **systemd**
being the biggest change
in CentOS / RHEL 7.
