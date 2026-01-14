# Additional Cron Jobs (hourly, daily, weekly, monthly)

Linux provides predefined directories
to run scheduled tasks automatically
at common time intervals.

## Cron directories
- `/etc/cron.hourly`  – run tasks every hour
- `/etc/cron.daily`   – run tasks once per day
- `/etc/cron.weekly`  – run tasks once per week
- `/etc/cron.monthly` – run tasks once per month

## How it works
- Scripts placed in these directories
  are executed by the system cron service
- Scripts must be executable

## Example
- Add a script to run daily:
- `cp myscript.sh /etc/cron.daily/`
- `chmod +x /etc/cron.daily/myscript.sh`

## Notes
- Execution time is controlled by `/etc/crontab`
- No need to edit user crontabs for these jobs

These cron directories simplify
system-wide scheduled task management.
