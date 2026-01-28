## Central Logger (rsyslog)

rsyslog is a powerful
logging service used
to collect, store,
and forward system logs.

### Key Features
- Centralized log management
- Supports TCP and UDP
- Reliable and scalable
- Default logging service on Linux

### Install rsyslog
```bash
dnf install rsyslog -y
```

### Start and Enable Service
```bash
systemctl enable --now rsyslog
```

### Main Configuration File
- `/etc/rsyslog.conf`
- `/etc/rsyslog.d/`

### Enable Log Reception (Server)
```text
module(load="imudp")
input(type="imudp" port="514")

module(load="imtcp")
input(type="imtcp" port="514")
```

### Client Configuration (Forward Logs)
```text
*.* @@logserver_ip:514
```

### Firewall Configuration
```bash
firewall-cmd --add-port=514/udp --permanent
firewall-cmd --add-port=514/tcp --permanent
firewall-cmd --reload
```

### Summary
rsyslog enables centralized
logging, making monitoring,
troubleshooting, and auditing
more efficient in Linux systems.
