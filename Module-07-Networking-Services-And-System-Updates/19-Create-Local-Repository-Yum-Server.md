## Create Local Repository (YUM Server)

A local YUM repository allows
systems to install packages
without internet access.

### Requirements
- Linux system with storage
- RPM packages
- `createrepo` package
- Web server (httpd)

### Install Required Packages
```bash
dnf install createrepo httpd -y
```

### Create Repository Directory
```bash
mkdir -p /var/www/html/localrepo
```

### Copy RPM Packages
```bash
cp *.rpm /var/www/html/localrepo/
```

### Create Repository Metadata
```bash
createrepo /var/www/html/localrepo
```

### Start Web Server
```bash
systemctl enable --now httpd
```

### Create Repo File on Client
```bash
vi /etc/yum.repos.d/local.repo
```

Example:
```ini
[localrepo]
name=Local YUM Repo
baseurl=http://server_ip/localrepo
enabled=1
gpgcheck=0
```

### Clean and Test
```bash
dnf clean all
dnf repolist
```

### Summary
A local YUM repository
provides controlled package
management and is commonly
used in enterprise environments.
