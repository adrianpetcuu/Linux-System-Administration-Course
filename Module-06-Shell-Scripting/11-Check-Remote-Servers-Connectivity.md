# Check Remote Servers Connectivity

Linux provides several commands
to verify network connectivity
and reachability of remote servers.

## ping
- Tests basic network connectivity
- Sends ICMP echo requests
- Example:
```
ping google.com
```

## traceroute
- Displays the path packets take
  to reach a remote host
- Useful for diagnosing network issues
- Example:
```
traceroute google.com
```

## ssh
- Tests remote access and authentication
- Confirms service and port availability
- Example:
```
ssh user@remote_server
```

## nc (netcat)
- Checks if a specific port is open
- Example:
```
nc -zv server_ip 22
```

## curl / wget
- Tests HTTP/HTTPS connectivity
- Example:
```
curl http://example.com
```

Checking remote server connectivity
is essential for troubleshooting
network and service availability.
