# at Command

The `at` command is used
to schedule a one-time task
to run at a specific time in Linux.

## When to use at
- Run a command once in the future
- Not suitable for recurring jobs
- Use `cron` for repetitive tasks

## Basic usage
- `at TIME`
- Enter commands interactively
- Press `Ctrl + D` to submit the job

## Examples
- Run a command at 10:30:
```
at 10:30
```
- Run a script tomorrow:
```
at tomorrow
```
- Run a command at a specific date and time:
```
at 18:00 2026-01-20
```

## Manage at jobs
- `atq` – list scheduled jobs
- `atrm JOB_ID` – remove a scheduled job

## Service requirement
- The `atd` service must be running:
```
systemctl status atd
```

The `at` command
is useful for delayed,
one-time task execution.
