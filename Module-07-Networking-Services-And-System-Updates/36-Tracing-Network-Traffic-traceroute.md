## Tracing Network Traffic (traceroute)

The `traceroute` command is used
to trace the path that packets take
from a source system to a destination
across a network.

### Purpose
- Identify network path hops
- Diagnose routing issues
- Measure latency between hops

### Install traceroute
```bash
dnf install traceroute -y
```

### Basic Usage
```bash
traceroute google.com
```

### Trace Using IP Address
```bash
traceroute 8.8.8.8
```

### How It Works
- Sends packets with increasing TTL values
- Each router decreases TTL by 1
- When TTL reaches zero, a response is sent back

### Common Output Information
- Hop number
- Router IP or hostname
- Response time (latency)

### Summary
`traceroute` helps administrators
visualize network paths and
troubleshoot connectivity and
routing problems.
