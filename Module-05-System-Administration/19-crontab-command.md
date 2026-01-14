# crontab Command

The `crontab` command is used
to schedule recurring tasks
to run automatically in Linux.

## Basic usage
- `crontab -e` – edit user crontab
- `crontab -l` – list scheduled jobs
- `crontab -r` – remove all cron jobs

## Cron time format
```
* * * * *
│ │ │ │ │
│ │ │ │ └─ day of week (0–7)
│ │ │ └─── month (1–12)
│ │ └───── day of month (1–31)
│ └─────── hour (0–23)
└───────── minute (0–59)
```

## Example
- Run a script every day at 02:00:
```
0 2 * * * /path/script.sh
```

## Special values
- `@reboot` – run at system startup
- `@daily` – run once per day
- `@weekly` – run once per week

The `crontab` command
is essential for task automation
and system maintenance.
