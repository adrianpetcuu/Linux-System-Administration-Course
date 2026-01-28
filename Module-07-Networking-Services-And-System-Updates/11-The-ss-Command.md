## The ss Command

The `ss` command is used
to display detailed information
about network sockets and connections.
It replaces the older `netstat` tool.

### Basic Usage
```bash
ss
```

### Show Listening Ports
```bash
ss -l
```

### Show TCP and UDP Sockets
```bash
ss -tuln
```

### Show Processes Using Ports
```bash
ss -tulnp
```

### Filter by Port
```bash
ss -tulnp | grep :22
```

### Common Options
- `-t` TCP sockets
- `-u` UDP sockets
- `-l` Listening sockets
- `-n` Do not resolve names
- `-p` Show process using the socket

### Summary
The `ss` command is a fast
and powerful tool for checking
open ports, active connections,
and network services.
