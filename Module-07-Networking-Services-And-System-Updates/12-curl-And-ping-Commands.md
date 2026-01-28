## curl and ping Command

The `curl` and `ping` commands
are commonly used to test
network connectivity and services.

### ping Command
- Tests basic network connectivity
- Uses ICMP protocol

```bash
ping google.com
ping -c 4 8.8.8.8
```

### curl Command
- Transfers data from or to a server
- Commonly used to test HTTP/HTTPS services

```bash
curl http://example.com
curl -I http://example.com
```

### Key Differences
- `ping` tests network reachability
- `curl` tests application-level services

### Summary
`ping` verifies network access,
while `curl` confirms that
a specific service is reachable
and responding correctly.
