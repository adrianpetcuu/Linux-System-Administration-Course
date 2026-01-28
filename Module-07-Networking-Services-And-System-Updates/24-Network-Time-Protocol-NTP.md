## Network Time Protocol (NTP)

Network Time Protocol (NTP)
is used to synchronize system
time with remote time servers.

### Modern NTP Implementation
- `chrony` is the default NTP client/server
- Replaces legacy `ntpd`

### Install Chrony
```bash
dnf install chrony -y
```

### Start and Enable Service
```bash
systemctl enable --now chronyd
```

### Configuration File
- `/etc/chrony.conf`

### Check Time Synchronization
```bash
chronyc sources
chronyc tracking
```

### Firewall (if acting as NTP server)
```bash
firewall-cmd --add-service=ntp --permanent
firewall-cmd --reload
```

### Summary
NTP ensures accurate system time,
which is critical for logs,
security, authentication,
and distributed systems.
