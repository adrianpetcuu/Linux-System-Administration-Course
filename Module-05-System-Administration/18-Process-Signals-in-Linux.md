# Process Signals in Linux

Process signals are notifications
sent to running processes
to control their behavior.

## What are signals
- Signals are used to stop, pause, resume,
  or reload processes
- Each signal has a name and a number
- Signals are sent using the `kill` command

## Common Linux signals
- `SIGTERM (15)` – request graceful termination
- `SIGKILL (9)` – forcefully stop a process
- `SIGHUP (1)` – reload configuration
- `SIGINT (2)` – interrupt process (Ctrl + C)
- `SIGSTOP (19)` – pause a process
- `SIGCONT (18)` – resume a paused process

## Examples
- `kill -15 PID`
- `kill -9 PID`
- `kill -HUP PID`
- `kill -STOP PID`
- `kill -CONT PID`

Understanding process signals
is essential for troubleshooting
and process management in Linux.
