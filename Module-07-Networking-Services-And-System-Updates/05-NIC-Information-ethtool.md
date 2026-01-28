## NIC Information (ethtool)

Network Interface Card (NIC) information
can be viewed and managed using the
`ethtool` command in Linux.

### What is ethtool
- Utility for querying and controlling NIC settings
- Displays speed, duplex, and link status
- Useful for troubleshooting network issues

### Check NIC details
```bash
ethtool enp0s3
```

### Common information shown
- Link detected (yes/no)
- Speed (e.g. 1000Mb/s)
- Duplex mode (Full/Half)
- Auto-negotiation status

### Change NIC settings (temporary)
```bash
ethtool -K enp0s3 tso off
```

### Notes
- Requires root privileges
- Changes are not persistent after reboot

### Summary
The `ethtool` command helps administrators
inspect and troubleshoot network interface
hardware and link-level settings.
