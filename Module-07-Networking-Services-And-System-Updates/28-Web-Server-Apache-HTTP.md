## Web Server Apache HTTP

Apache HTTP Server is a
widely used open-source
web server for hosting
websites and web applications.

### Key Features
- Serves HTTP and HTTPS content
- Supports virtual hosts
- Highly configurable and modular
- Stable and widely adopted

### Install Apache
```bash
dnf install httpd -y
```

### Start and Enable Service
```bash
systemctl enable --now httpd
```

### Main Configuration Files
- `/etc/httpd/conf/httpd.conf`
- `/etc/httpd/conf.d/`

### Document Root
- Default location:
```text
/var/www/html
```

### Firewall Configuration
```bash
firewall-cmd --add-service=http --permanent
firewall-cmd --reload
```

### Test Apache
Open in browser:
```
http://server_ip
```

### Summary
Apache HTTP Server provides
reliable web hosting and is
commonly used in enterprise
and Linux environments.
