## FTP File Transfer Protocol

FTP (File Transfer Protocol)
is used to transfer files
between a client and a server
over a network.

### Key Characteristics
- Uses TCP protocol
- Default port: 21
- Supports upload and download
- Not encrypted by default

### FTP Modes
- Active mode
- Passive mode

### FTP Client Example
```bash
ftp server_ip
```

### Common FTP Commands
- `ls` – list files
- `get` – download file
- `put` – upload file
- `bye` – exit session

### Security Note
FTP sends data and credentials
in plain text and is not secure.
SFTP or SCP is recommended instead.

### Summary
FTP allows file transfers
between systems but should
only be used in trusted
or legacy environments.
