## DNS Download, Install and Configure (Domain Name System)

DNS (Domain Name System)
translates domain names
into IP addresses.

### Install DNS Server (BIND)
```bash
dnf install bind bind-utils -y
```

### Main Configuration Files
- `/etc/named.conf`
- `/var/named/`

### Start and Enable DNS Service
```bash
systemctl enable --now named
```

### Configure Firewall
```bash
firewall-cmd --add-service=dns --permanent
firewall-cmd --reload
```

### Test DNS Resolution
```bash
dig google.com
nslookup google.com
```

### Local DNS Configuration
Edit resolver file:
```bash
vi /etc/resolv.conf
```

Example:
```text
nameserver 192.168.0.164
```

### Summary
DNS provides name resolution
services and is essential
for network communication
in Linux environments.
