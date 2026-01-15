# User and Global Aliases

Linux allows aliases
to be defined per user
or system-wide for all users.

## User aliases
- Available only for a specific user
- Defined in:
  - `~/.bashrc`
  - `~/.bash_aliases`

## Example user alias
```
alias ll='ls -lh'
```

## Global aliases
- Available for all users on the system
- Defined in:
  - `/etc/bashrc`
  - `/etc/profile`
  - `/etc/profile.d/*.sh`

## Example global alias
```
alias ll='ls -l'
```

## Apply changes
- Reload configuration:
```
source ~/.bashrc
```

User and global aliases
help standardize commands
and improve productivity
across the system.
