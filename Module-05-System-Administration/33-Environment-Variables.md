# Environment Variables

Environment variables are key-value pairs
that define the behavior of the shell
and applications in Linux.

## Common environment variables
- `PATH` – directories searched for commands
- `HOME` – user home directory
- `USER` – current logged-in user
- `SHELL` – default shell
- `LANG` – system language and locale

## View environment variables
- `env`
- `printenv`
- `echo $VARIABLE`

## Set environment variables
- Temporary (current session):
```
export VAR=value
```
- Permanent (user):
  - Add to `~/.bashrc` or `~/.bash_profile`
- Permanent (system-wide):
  - Add to `/etc/environment`

Environment variables are essential
for shell configuration, scripting,
and application behavior.
