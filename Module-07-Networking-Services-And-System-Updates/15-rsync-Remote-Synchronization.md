## rsync Remote Synchronization

rsync is a fast and efficient
tool used to synchronize files
and directories locally or
between remote systems.

### Key Characteristics
- Transfers only changed data
- Uses SSH for secure transfer
- Preserves permissions and ownership
- Suitable for backups and mirroring

### Local Synchronization
```bash
rsync -av source/ destination/
```

### Remote Synchronization
```bash
rsync -av source/ user@server_ip:/path/
```

### Copy from Remote Server
```bash
rsync -av user@server_ip:/path/ /local/path/
```

### Common Options
- `-a` archive mode
- `-v` verbose
- `-z` compress data
- `--delete` remove deleted files from destination

### Summary
rsync is a powerful tool
for efficient and secure
file synchronization and
backup operations.
