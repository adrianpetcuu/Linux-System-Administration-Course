## DHCP Server

DHCP (Dynamic Host Configuration Protocol)
automatically assigns IP addresses
and network configuration to clients.

### Key Features
- Automatic IP address allocation
- Reduces manual configuration
- Centralized network management

### Install DHCP Server
```bash
dnf install dhcp-server -y
```

### Main Configuration File
- `/etc/dhcp/dhcpd.conf`

### Basic DHCP Configuration Example
```text
subnet 192.168.1.0 netmask 255.255.255.0 {
  range 192.168.1.100 192.168.1.200;
  option routers 192.168.1.1;
  option domain-name-servers 8.8.8.8;
}
```

### Start and Enable DHCP Service
```bash
systemctl enable --now dhcpd
```

### Firewall Configuration
```bash
firewall-cmd --add-service=dhcp --permanent
firewall-cmd --reload
```

### Check Service Status
```bash
systemctl status dhcpd
```

### Summary
DHCP servers simplify
network administration by
automatically providing IP
configuration to clients.
