## SSH and Telnet

SSH and Telnet are remote
access protocols used to
connect to Linux systems.

### SSH (Secure Shell)
- Secure and encrypted
- Default port: 22
- Used for remote administration
- Supports authentication and encryption

Example:
```bash
ssh user@server_ip
```

### Telnet
- Unencrypted and insecure
- Default port: 23
- Not recommended for production use
- Mostly obsolete

Example:
```bash
telnet server_ip
```

### Key Differences
- SSH encrypts data; Telnet does not
- SSH is secure; Telnet is insecure
- SSH is widely used; Telnet is deprecated

### Summary
SSH is the standard tool
for secure remote access,
while Telnet is only used
for legacy or testing purposes.
