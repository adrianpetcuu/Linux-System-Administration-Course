## Network Files and Commands

Linux networking is managed using configuration files and command-line tools for testing, monitoring, and troubleshooting.

### Network Configuration Files
- **/etc/sysconfig/network-scripts/** – Legacy network interface configs (RHEL/CentOS)
- **/etc/NetworkManager/** – NetworkManager configuration
- **/etc/resolv.conf** – DNS resolver configuration
- **/etc/hosts** – Static hostname-to-IP mappings

### ping
- Tests network connectivity using ICMP
```bash
ping google.com
ping -c 4 8.8.8.8
```

### ifup / ifdown
- Brings a network interface up or down (legacy systems)
```bash
ifup enp0s3
ifdown enp0s3
```

### netstat
- Displays network connections, routing tables, and listening ports
```bash
netstat -tulnp
netstat -rn
```

### tcpdump
- Captures and analyzes network packets
```bash
tcpdump -i enp0s3
tcpdump -n port 80
```

### Summary
Network files define how interfaces and DNS work, while commands like `ping`, `ifup/ifdown`, `netstat`, and `tcpdump` help test connectivity and troubleshoot network issues.
