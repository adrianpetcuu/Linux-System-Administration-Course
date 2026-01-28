## Enable Internet on Linux VM

To enable internet access on a Linux Virtual Machine (VM), the network must be properly configured both in the **hypervisor** and inside the **Linux OS**.

### Common Network Modes (VirtualBox)
- **NAT** – Easiest setup, internet works automatically
- **Bridged Adapter** – VM gets an IP from the same network as the host
- **Host-Only** – Communication only with host (no internet by default)

### Basic Steps
1. **Configure Network Adapter**
   - Set adapter to **NAT** or **Bridged**

2. **Ensure Network Service is Running**
```bash
systemctl status NetworkManager
systemctl start NetworkManager
systemctl enable NetworkManager
```

3. **Check Network Interface**
```bash
ip a
nmcli device status
```

4. **Verify IP Address**
```bash
ip addr show
```
The interface should have an IP address (DHCP).

### Test Internet Connectivity
```bash
ping -c 3 8.8.8.8
ping -c 3 google.com
```

### DNS Configuration (if needed)
```bash
cat /etc/resolv.conf
```

Example:
```text
nameserver 8.8.8.8
```

### Firewall Check
Ensure outbound traffic is allowed:
```bash
firewall-cmd --state
```

### Common Issues
- Network interface is down
- Wrong adapter mode selected
- Missing or incorrect DNS
- Firewall blocking traffic

### Summary
Internet access on a Linux VM depends on correct adapter mode, active network interface, valid IP address, and proper DNS configuration.
