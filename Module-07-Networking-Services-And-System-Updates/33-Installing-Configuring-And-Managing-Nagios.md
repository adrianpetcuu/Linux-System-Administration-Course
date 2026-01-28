## Installing, Configuring and Managing Nagios

Nagios is a monitoring
system used to monitor
hosts, services, and
network infrastructure.

### Install Required Packages
```bash
dnf install httpd php gcc glibc glibc-common -y
dnf install nagios nagios-plugins-all -y
```

### Start and Enable Services
```bash
systemctl enable --now httpd
systemctl enable --now nagios
```

### Main Configuration Files
- `/etc/nagios/nagios.cfg`
- `/etc/nagios/conf.d/`

### Web Interface
- Default URL:
```
http://server_ip/nagios
```

### Authentication
- Uses Apache basic authentication
- Users stored in:
  - `/etc/nagios/passwd`

### Check Configuration
```bash
nagios -v /etc/nagios/nagios.cfg
```

### Firewall Configuration
```bash
firewall-cmd --add-service=http --permanent
firewall-cmd --reload
```

### Summary
Nagios provides centralized
monitoring of systems
and services and is widely
used in enterprise environments.
