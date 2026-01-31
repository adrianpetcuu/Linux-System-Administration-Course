## Difference Between CentOS and RHEL 7 & 8

CentOS and Red Hat Enterprise Linux (RHEL)
are closely related enterprise Linux
distributions, but differences exist
between versions 7 and 8.

---

## RHEL / CentOS 7
- Released in 2014
- Uses **systemd**
- XFS default filesystem
- Python 2 system Python
- yum package manager
- Stable, long-term enterprise release

Key commands:
```bash
systemctl
yum install
```

---

## RHEL / CentOS 8
- Released in 2019
- Uses **systemd** (improved)
- XFS default filesystem
- Python 3 system Python
- dnf package manager (replaces yum)
- Modular repositories (AppStreams)

Key commands:
```bash
systemctl
dnf install
```

---

## CentOS vs RHEL
- **RHEL**: Paid, supported by Red Hat
- **CentOS**: Free, community-supported
- Binary compatible (traditional CentOS)
- CentOS Stream = rolling preview of RHEL

---

## Key Differences Summary

| Feature | RHEL/CentOS 7 | RHEL/CentOS 8 |
|------|------|------|
| Init system | systemd | systemd |
| Package manager | yum | dnf |
| Python version | Python 2 | Python 3 |
| Repos | Classic | Modular (AppStreams) |
| Lifecycle | Longer | Modern stack |

---

## Summary
RHEL/CentOS 8 introduced
modern tooling, DNF, and
Python 3, while maintaining
enterprise stability compared
to RHEL/CentOS 7.
