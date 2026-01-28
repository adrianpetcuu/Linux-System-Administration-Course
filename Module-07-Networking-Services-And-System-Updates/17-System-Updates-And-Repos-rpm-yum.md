## System Updates and Repos (rpm, yum)

Linux systems use package managers
to install, update, and manage software
from repositories.

### rpm (Red Hat Package Manager)
- Low-level package management tool
- Installs individual `.rpm` files
- Does not resolve dependencies automatically

```bash
rpm -ivh package.rpm
rpm -qa
rpm -qi package_name
```

### yum (Yellowdog Updater Modified)
- High-level package manager
- Automatically resolves dependencies
- Uses repositories

```bash
yum install httpd
yum update
yum remove httpd
```

### Repository Files
- Located in:
  - `/etc/yum.repos.d/`
- Define software sources

### Key Differences
- `rpm` works with local packages
- `yum` works with repositories and dependencies

### Summary
rpm manages individual packages,
while yum simplifies software
management using repositories.
