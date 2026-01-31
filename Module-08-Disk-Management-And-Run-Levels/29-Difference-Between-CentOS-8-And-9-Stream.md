## Difference Between CentOS Stream 8 and CentOS Stream 9

CentOS Stream is a rolling-release
distribution that sits between
Fedora and RHEL, acting as a
preview of future RHEL releases.

---

## CentOS Stream 8
- Based on RHEL 8
- Uses **DNF**
- Python 3 by default
- Older kernel and userland
- End of life: May 2024

Typical use:
- Labs
- Legacy testing
- RHEL 8 preview (historical)

---

## CentOS Stream 9
- Based on RHEL 9
- Uses **DNF** (improved)
- Newer kernel (5.x+)
- Modern toolchain (GCC, glibc)
- Stronger security defaults
- Actively supported

Typical use:
- New deployments
- Modern labs
- RHEL 9 preview

---

## Key Differences Summary

| Feature | Stream 8 | Stream 9 |
|------|---------|---------|
| RHEL base | RHEL 8 | RHEL 9 |
| Status | EOL | Active |
| Kernel | Older | Newer |
| Security | Standard | Enhanced |
| Use case | Legacy | Modern |

---

## Important Notes
- Stream is **rolling**, not fixed
- Not recommended for strict production
- Best for learning and testing RHEL features

---

## Summary
CentOS Stream 9 is the
modern and supported
choice, while Stream 8
is deprecated and should
only be used for legacy
testing purposes.
