## Tune System Performance (tuned, nice, renice)

Linux provides tools
to optimize system performance
by managing resource usage
and process priorities.

### tuned
- System tuning daemon
- Applies performance profiles
- Optimizes CPU, disk, and network

Install and start:
```bash
dnf install tuned -y
systemctl enable --now tuned
```

Check active profile:
```bash
tuned-adm active
```

List available profiles:
```bash
tuned-adm list
```

Set a profile:
```bash
tuned-adm profile throughput-performance
```

---

### nice
- Sets process priority at start
- Priority range: -20 (highest) to 19 (lowest)

Example:
```bash
nice -n 10 command
```

---

### renice
- Changes priority of running process

Example:
```bash
renice -n 5 -p PID
```

---

### Summary
`tuned` optimizes system-wide
performance using profiles,
while `nice` and `renice`
control CPU priority for
individual processes.
