# System Logs Monitoring – /var/log

Linux stores system and application
log files inside the `/var/log`
directory for troubleshooting
and auditing purposes.

## Common log files
- `/var/log/messages` – general system messages
- `/var/log/syslog` – system activity logs (Debian-based)
- `/var/log/secure` – authentication and security logs
- `/var/log/boot.log` – system boot messages
- `/var/log/cron` – cron job activity
- `/var/log/dmesg` – kernel-related messages

## Log monitoring commands
- `cat logfile` – display log content
- `less logfile` – view logs page by page
- `tail logfile` – view last lines
- `tail -f logfile` – monitor logs in real time
- `grep keyword logfile` – search logs

## Examples
- `tail -f /var/log/messages`
- `grep ssh /var/log/secure`

System log monitoring
is essential for diagnosing
errors, security events,
and system behavior.
