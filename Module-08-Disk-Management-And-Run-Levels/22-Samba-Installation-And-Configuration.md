## Samba Installation and Configuration

Samba allows Linux systems
to share files and printers
with Windows systems using
the SMB/CIFS protocol.

---

### Install Samba
```bash
dnf install samba samba-client samba-common -y
```

---

### Main Configuration File
- `/etc/samba/smb.conf`

---

### Basic Samba Share Configuration
Edit configuration:
```bash
vi /etc/samba/smb.conf
```

Example share:
```text
[shared]
  path = /samba/share
  writable = yes
  browseable = yes
  guest ok = no
```

---

### Create Shared Directory
```bash
mkdir -p /samba/share
chmod 777 /samba/share
```

---

### Create Samba User
```bash
useradd sambauser
smbpasswd -a sambauser
```

---

### Start and Enable Samba
```bash
systemctl enable --now smb nmb
```

---

### Firewall Configuration
```bash
firewall-cmd --add-service=samba --permanent
firewall-cmd --reload
```

---

### Verify Samba
```bash
smbclient -L localhost
```

---

### Summary
Samba enables seamless
file sharing between Linux
and Windows systems and is
widely used in mixed OS
environments.
