## systemd-analyze Command

The `systemd-analyze` command is used
to analyze system boot performance
and identify slow services during startup.

### Purpose
- Measure boot time
- Identify performance bottlenecks
- Analyze service startup order

### Show Total Boot Time
```bash
systemd-analyze
```

Output includes:
- Firmware time
- Bootloader time
- Kernel time
- Userspace time

### List Services by Startup Time
```bash
systemd-analyze blame
```

### Show Dependency Tree
```bash
systemd-analyze critical-chain
```

### Analyze Specific Service
```bash
systemd-analyze critical-chain sshd.service
```

### Generate Boot Graph (Optional)
```bash
systemd-analyze plot > boot.svg
```

### Summary
`systemd-analyze` helps administrators
optimize boot performance by identifying
slow services and understanding the
system startup process.
