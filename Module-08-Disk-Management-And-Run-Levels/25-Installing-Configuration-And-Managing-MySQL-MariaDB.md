## Installing, Configuring and Managing MySQL / MariaDB

MySQL and MariaDB are
relational database management
systems (RDBMS) used to store
and manage structured data.

MariaDB is a community-driven
fork of MySQL and is the default
on many Linux distributions.

---

## Install MariaDB (Recommended on RHEL/CentOS)

```bash
dnf install mariadb-server mariadb -y
```

---

## Start and Enable Service

```bash
systemctl enable --now mariadb
```

Check status:
```bash
systemctl status mariadb
```

---

## Secure Installation

```bash
mysql_secure_installation
```

This allows you to:
- Set root password
- Remove anonymous users
- Disable remote root login
- Remove test database

---

## Login to Database

```bash
mysql -u root -p
```

---

## Basic Database Management

Create database:
```sql
CREATE DATABASE mydb;
```

Create user:
```sql
CREATE USER 'dbuser'@'localhost' IDENTIFIED BY 'password';
```

Grant privileges:
```sql
GRANT ALL PRIVILEGES ON mydb.* TO 'dbuser'@'localhost';
FLUSH PRIVILEGES;
```

---

## Configuration File
- `/etc/my.cnf`
- `/etc/my.cnf.d/`

Restart after changes:
```bash
systemctl restart mariadb
```

---

## Firewall (Optional – Remote Access)

```bash
firewall-cmd --add-service=mysql --permanent
firewall-cmd --reload
```

---

## Summary
MySQL / MariaDB provide
reliable relational database
services and are widely used
in web applications and
enterprise environments.
