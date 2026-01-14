# System Monitoring Commands

Linux provides monitoring commands
to check disk usage, memory,
CPU, hardware messages, and networking.

## df
- Displays disk space usage
- Common option:
  - `df -h` – human-readable output

## dmesg
- Shows kernel ring buffer messages
- Useful for hardware and boot issues
- Example: `dmesg | less`

## iostat
- Displays CPU and disk I/O statistics
- Requires `sysstat` package
- Example: `iostat 1`

## netstat
- Displays network connections and ports
- Common options:
  - `-tulpn` – listening ports and services
- Example: `netstat -tulpn`

## free
- Displays memory usage
- Example: `free -h`

## top
- Real-time process and resource monitoring
- Shows CPU, memory, and running processes

These commands are essential
for monitoring system health
and troubleshooting performance issues.
