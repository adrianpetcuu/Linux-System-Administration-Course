# The screen Command

The `screen` command is a terminal multiplexer
that allows multiple shell sessions
inside a single terminal window.

## Why use screen
- Keep processes running after logout
- Work with multiple terminals in one session
- Useful for long-running tasks

## Basic usage
- Start a screen session:
```
screen
```
- Detach from session:
```
Ctrl + a  d
```
- Reattach session:
```
screen -r
```

## Common screen commands
- `Ctrl + a  c` – create a new window
- `Ctrl + a  n` – next window
- `Ctrl + a  p` – previous window
- `Ctrl + a  "` – list windows
- `Ctrl + a  S` – split screen horizontally
- `Ctrl + a  Tab` – switch between panes
- `Ctrl + a  Q` – close split

## List screen sessions
```
screen -ls
```

The `screen` command
is commonly used by system administrators
and is useful for RHCSA exams.
