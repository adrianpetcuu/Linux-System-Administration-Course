## Kickstart – Automate Linux Installation

Kickstart is a method
used to automate Linux
installations by using
a predefined configuration file.

### Key Benefits
- Fully automated OS installation
- Consistent system configuration
- Saves time in large deployments
- Widely used in enterprise environments

### Kickstart File
- Configuration file: `ks.cfg`
- Defines installation options:
  - Language, timezone
  - Disk partitioning
  - Packages
  - Network settings
  - Root password

### Basic Kickstart Example
```text
install
url --url=http://mirror.centos.org/centos/
lang en_US.UTF-8
keyboard us
timezone Europe/Bucharest
rootpw password
reboot
```

### Using Kickstart
- Provide `ks.cfg` during boot
- Boot option example:
```text
inst.ks=http://server_ip/ks.cfg
```

### Common Usage
- PXE network installations
- Virtual machine provisioning
- Data center automation

### Summary
Kickstart automates Linux
installations using a single
configuration file, ensuring
speed, consistency, and scalability.
