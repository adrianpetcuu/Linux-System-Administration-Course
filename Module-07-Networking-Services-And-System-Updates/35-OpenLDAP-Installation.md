## OpenLDAP Installation

OpenLDAP is an open-source
directory service used
for centralized authentication
and user management.

### Install OpenLDAP Packages
```bash
dnf install openldap openldap-servers openldap-clients -y
```

### Enable and Start Service
```bash
systemctl enable --now slapd
```

### Main Configuration Directory
- `/etc/openldap/`
- `/var/lib/ldap/`

### Check Service Status
```bash
systemctl status slapd
```

### Firewall Configuration
```bash
firewall-cmd --add-service=ldap --permanent
firewall-cmd --reload
```

### Test LDAP Service
```bash
ldapsearch -x
```

### Summary
OpenLDAP provides centralized
directory services for users,
groups, and authentication
in Linux environments.
