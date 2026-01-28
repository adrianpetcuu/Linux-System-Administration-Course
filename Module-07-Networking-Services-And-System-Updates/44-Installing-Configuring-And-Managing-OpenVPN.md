## Installing, Configuring and Managing OpenVPN

OpenVPN is an open-source
VPN solution used to create
secure encrypted tunnels
over untrusted networks.

### Key Features
- Secure remote access
- Uses SSL/TLS encryption
- Client-server architecture
- Widely used in enterprises

### Install OpenVPN
```bash
dnf install epel-release -y
dnf install openvpn -y
```

### Configuration Files
- Server config: `/etc/openvpn/server.conf`
- Client config: `/etc/openvpn/client.conf`

### Start and Enable OpenVPN
```bash
systemctl enable --now openvpn-server@server
```

### Firewall Configuration
```bash
firewall-cmd --add-service=openvpn --permanent
firewall-cmd --reload
```

### Check VPN Status
```bash
systemctl status openvpn-server@server
```

### Common Management Tasks
- Start/stop VPN service
- Manage certificates and keys
- Monitor VPN connections

### Summary
OpenVPN provides secure
remote connectivity and
encrypted communication
for Linux servers and clients.
