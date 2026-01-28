## Proxy Server in Linux (Squid)

Squid is a popular
proxy server used
to control, secure,
and optimize web traffic.

### Key Features
- Caching web content
- Access control policies
- Improves performance
- Enhances security

### Install Squid
```bash
dnf install squid -y
```

### Start and Enable Service
```bash
systemctl enable --now squid
```

### Main Configuration File
- `/etc/squid/squid.conf`

### Default Proxy Port
- 3128

### Basic Access Control Example
```text
http_access allow localhost
http_access deny all
```

### Firewall Configuration
```bash
firewall-cmd --add-port=3128/tcp --permanent
firewall-cmd --reload
```

### Test Proxy
Configure browser or system
to use proxy:
```
server_ip:3128
```

### Summary
Squid provides web proxy
and caching services
commonly used in enterprise
Linux environments.
