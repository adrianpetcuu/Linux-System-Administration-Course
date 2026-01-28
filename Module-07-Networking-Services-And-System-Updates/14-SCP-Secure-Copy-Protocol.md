## SCP Secure Copy Protocol

SCP (Secure Copy Protocol)
is used to securely transfer files
between systems over SSH.

### Key Characteristics
- Uses SSH for encryption
- Default port: 22
- Secure file transfer
- Supports local and remote copying

### Copy File to Remote Server
```bash
scp file.txt user@server_ip:/path/
```

### Copy File from Remote Server
```bash
scp user@server_ip:/path/file.txt /local/path/
```

### Copy Directories Recursively
```bash
scp -r directory/ user@server_ip:/path/
```

### Common Options
- `-r` copy directories recursively
- `-p` preserve file permissions
- `-C` enable compression

### Summary
SCP provides a simple
and secure method for
transferring files using
SSH encryption.
