## Installing, Configuring and Managing NGINX

NGINX is a high-performance
web server and reverse proxy
commonly used for web hosting
and load balancing.

### Install NGINX
```bash
dnf install nginx -y
```

### Start and Enable Service
```bash
systemctl enable --now nginx
```

### Main Configuration Files
- `/etc/nginx/nginx.conf`
- `/etc/nginx/conf.d/`

### Default Web Root
```text
/usr/share/nginx/html
```

### Test Configuration
```bash
nginx -t
```

### Reload or Restart NGINX
```bash
systemctl reload nginx
systemctl restart nginx
```

### Firewall Configuration
```bash
firewall-cmd --add-service=http --permanent
firewall-cmd --reload
```

### Test NGINX
Open in browser:
```
http://server_ip
```

### Summary
NGINX provides fast,
scalable web services
and is widely used
in modern Linux systems.
