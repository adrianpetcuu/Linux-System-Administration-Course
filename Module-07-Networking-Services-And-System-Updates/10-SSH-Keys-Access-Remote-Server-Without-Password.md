## SSH Keys Access Remote Server Without Password

SSH key-based authentication allows
secure access to remote servers
without using passwords.

### Generate SSH Key Pair
```bash
ssh-keygen
```

This creates:
- Private key: `~/.ssh/id_rsa`
- Public key: `~/.ssh/id_rsa.pub`

### Copy Public Key to Server
```bash
ssh-copy-id user@server_ip
```

### Login Without Password
```bash
ssh user@server_ip
```

### SSH Key Permissions
- Private key: `600`
- `.ssh` directory: `700`

```bash
chmod 700 ~/.ssh
chmod 600 ~/.ssh/id_rsa
```

### Disable Password Authentication (Optional)
Edit:
```text
/etc/ssh/sshd_config
```

Set:
```
PasswordAuthentication no
```

Restart SSH:
```bash
systemctl restart sshd
```

### Summary
SSH keys provide a secure
and convenient way to access
remote servers without passwords.
