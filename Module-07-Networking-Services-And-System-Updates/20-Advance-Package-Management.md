## Advanced Package Management

Advanced package management
involves controlling software
versions, repositories,
and troubleshooting issues.

### List Installed Packages
```bash
dnf list installed
```

### Search Packages
```bash
dnf search package_name
```

### Show Package Information
```bash
dnf info package_name
```

### Enable or Disable Repositories
```bash
dnf repolist
dnf config-manager --set-enabled repo_id
dnf config-manager --set-disabled repo_id
```

### Exclude Packages from Updates
```bash
dnf update --exclude=package_name
```

### Rollback Using History
```bash
dnf history
dnf history undo ID
```

### Clean Metadata and Cache
```bash
dnf clean all
```

### Summary
Advanced package management
helps administrators control
software updates, repositories,
and system stability.
