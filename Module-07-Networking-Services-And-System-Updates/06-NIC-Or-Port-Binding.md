## NIC or Port Binding

NIC or port binding is the process
of associating a service or application
with a specific network interface
or network port.

### NIC Binding
- Binds a service to a specific network interface
- Limits access to traffic from that interface only
- Improves security and traffic control

Example (listen on specific IP):
```bash
ss -tulnp
```

Configuration example:
```
Listen 192.168.0.164:80
```

### Port Binding
- Binds a service to a specific port number
- Ensures services do not conflict
- Common ports: 22 (SSH), 80 (HTTP), 443 (HTTPS)

Example:
```bash
ss -tulnp | grep :80
```

### Why Binding is Important
- Improves security
- Controls network access
- Prevents port conflicts
- Used in multi-interface servers

### Summary
NIC and port binding allow administrators
to control where services listen and
which network traffic they accept.
