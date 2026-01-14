# Switch Users and Sudo Access (su, sudo)

Linux provides commands
to switch between users
and perform administrative tasks.

## su command
- Switches to another user account
- Requires the target user’s password
- Commonly used to become root

## sudo command
- Executes commands with elevated privileges
- Requires the current user’s password
- Access is controlled by sudoers configuration

## Common examples
- `su -` – switch to root user
- `su - username` – switch to another user
- `sudo command` – run command as root
- `sudo -i` – open a root shell

Using `sudo` is safer
than direct root access
and is recommended for administration.
