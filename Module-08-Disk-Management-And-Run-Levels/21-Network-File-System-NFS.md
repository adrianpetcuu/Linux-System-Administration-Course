## Network File System (NFS)

NFS allows systems
to share directories
over a network as if
they were local filesystems.

---

### NFS Architecture
- **NFS Server** – exports directories
- **NFS Client** – mounts shared directories
- Uses client-server model

---

### Install NFS Server
```bash
dnf install nfs-utils -y
```

Enable services:
```bash
systemctl enable --now nfs-server
```

---

### Configure NFS Export
Edit:
```bash
vi /etc/exports
```

Example:
```text
/data 192.168.1.0/24(rw,sync,no_root_squash)
```

Apply configuration:
```bash
exportfs -rv
```

---

### Firewall Configuration
```bash
firewall-cmd --add-service=nfs --permanent
firewall-cmd --reload
```

---

### Mount NFS Share (Client)
```bash
mount server_ip:/data /mnt
```

Persistent mount:
```text
server_ip:/data /mnt nfs defaults 0 0
```

---

### Verify
```bash
showmount -e server_ip
df -h
```

---

### Summary
NFS enables centralized
file sharing across Linux
systems and is widely used
in enterprise environments.
