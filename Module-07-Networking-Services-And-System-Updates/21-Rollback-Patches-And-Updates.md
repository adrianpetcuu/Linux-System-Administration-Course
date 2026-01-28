## Rollback Patches and Updates

Rollback allows administrators
to revert system changes
after updates or patches
cause issues.

### Using dnf History
DNF keeps a history
of all package transactions.

```bash
dnf history
```

### View Transaction Details
```bash
dnf history info ID
```

### Undo a Transaction
```bash
dnf history undo ID
```

### Rollback to a Previous State
```bash
dnf history rollback ID
```

### Kernel Rollback
- Multiple kernels are kept installed
- Select older kernel at boot (GRUB)

### Best Practices
- Always review changes before rollback
- Test rollback in non-production systems
- Keep backups before major updates

### Summary
Rollback mechanisms help
restore system stability
by reversing problematic
patches or updates.
