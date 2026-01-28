## Hostname or IP Lookup (nslookup and dig)

Linux provides tools to
query DNS servers and
resolve hostnames and IPs.

### nslookup
- Simple DNS query tool
- Used for quick lookups

```bash
nslookup google.com
nslookup 8.8.8.8
```

### dig
- Advanced DNS diagnostic tool
- Provides detailed query information

```bash
dig google.com
dig @8.8.8.8 google.com
```

### Common Uses
- Resolve hostname to IP
- Resolve IP to hostname (reverse lookup)
- Troubleshoot DNS issues

### Differences
- `nslookup` is simple and interactive
- `dig` is more detailed and script-friendly

### Summary
`nslookup` and `dig` are
essential tools for DNS
testing and troubleshooting
in Linux systems.
