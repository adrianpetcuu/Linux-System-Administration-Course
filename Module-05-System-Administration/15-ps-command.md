# ps Command

The `ps` command is used
to display information
about running processes.

## Common usage
- `ps` – show processes in current shell
- `ps -e` – show all running processes
- `ps -f` – full format listing
- `ps aux` – detailed view of all processes

## Important columns
- PID – process ID
- USER – process owner
- %CPU – CPU usage
- %MEM – memory usage
- COMMAND – executed command

## Examples
- `ps -ef | grep sshd`
- `ps aux | grep root`

The `ps` command
is essential for process monitoring
and troubleshooting.
