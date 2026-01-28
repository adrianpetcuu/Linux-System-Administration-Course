## Firewall in Linux

A firewall is a security system
that controls incoming and outgoing
network traffic based on rules.
In Linux, the firewall protects
the system from unauthorized access.

### firewalld (Default Firewall)
- Dynamic firewall management tool
- Uses zones to define trust levels
- Default on RHEL, CentOS, Fedora

### Firewall Zones
Zones define how much traffic is allowed:
- **public** – default, untrusted networks
- **trusted** – all traffic allowed
- **internal** – internal networks
- **drop** – drops all incoming traffic
- **block** – blocks and rejects traffic

Check active zones:
```bash
firewall-cmd --get-active-zones
```

### Basic Firewall Commands
Start and enable firewall:
```bash
systemctl enable --now firewalld
```

Check firewall status:
```bash
firewall-cmd --state
```

List current rules:
```bash
firewall-cmd --list-all
```

### Allow Services and Ports
Allow a service:
```bash
firewall-cmd --add-service=ssh --permanent
```

Allow a port:
```bash
firewall-cmd --add-port=8080/tcp --permanent
```

Apply changes:
```bash
firewall-cmd --reload
```

### Remove Services or Ports
```bash
firewall-cmd --remove-service=http --permanent
firewall-cmd --remove-port=8080/tcp --permanent
firewall-cmd --reload
```

### ICMP (Ping) Control
Block ping requests:
```bash
firewall-cmd --add-icmp-block=echo-request --permanent
firewall-cmd --reload
```

### Interface and Zone Binding
Assign interface to a zone:
```bash
firewall-cmd --zone=public --change-interface=enp0s3 --permanent
firewall-cmd --reload
```

### Runtime vs Permanent Rules
- **Runtime** rules: active until reboot
- **Permanent** rules: survive reboot

View runtime rules:
```bash
firewall-cmd --list-all
```

View permanent rules:
```bash
firewall-cmd --list-all --permanent
```

### Why Firewall Is Critical
- Blocks unauthorized access
- Limits exposed services
- Protects against network attacks
- Required for server security

### Summary
The Linux firewall is a core
security component that controls
network access using zones,
services, ports, and rules.
Proper firewall configuration
is essential for production systems.
