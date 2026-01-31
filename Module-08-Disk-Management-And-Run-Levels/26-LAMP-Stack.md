## LAMP Stack

LAMP is a popular web
application stack used
to host dynamic websites
and web applications.

LAMP stands for:
- **Linux**
- **Apache**
- **MySQL / MariaDB**
- **PHP**

---

## Components Overview

### Linux
- Operating system
- Provides stability and security

### Apache
- Web server
- Handles HTTP requests

### MySQL / MariaDB
- Database server
- Stores application data

### PHP
- Server-side scripting language
- Generates dynamic web content

---

## Install LAMP Stack (RHEL/CentOS)

```bash
dnf install httpd mariadb-server php php-mysqlnd -y
```

---

## Start and Enable Services

```bash
systemctl enable --now httpd mariadb
```

---

## Secure Database

```bash
mysql_secure_installation
```

---

## Test PHP

Create test file:
```bash
vi /var/www/html/info.php
```

Add:
```php
<?php phpinfo(); ?>
```

Access in browser:
```
http://server_ip/info.php
```

---

## Firewall Configuration

```bash
firewall-cmd --add-service=http --permanent
firewall-cmd --reload
```

---

## Summary
LAMP is a complete
web hosting stack widely
used for Linux-based
web applications.
