## chronyd – New Version of NTP

chronyd is the modern
implementation of NTP
used on RHEL, CentOS,
and Fedora systems.

### What is chronyd
- Replacement for legacy `ntpd`
- Faster time synchronization
- Works well on VMs and laptops

### Install chrony
```bash
dnf install chrony -y
```

### Start and Enable Service
```bash
systemctl enable --now chronyd
```

### Configuration File
- `/etc/chrony.conf`

### Check Synchronization Status
```bash
chronyc sources
chronyc tracking
```

### Advantages Over ntpd
- Faster convergence
- Better handling of network changes
- Lower resource usage

### Summary
chronyd is the preferred
time synchronization service
for modern Linux systems.
