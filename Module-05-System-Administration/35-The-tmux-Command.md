# The tmux Command

The `tmux` command is a terminal multiplexer
that allows multiple terminal sessions
inside a single window.

## Why use tmux
- Detach and reattach sessions
- Split terminal into panes
- Keep processes running after logout
- Preferred tool in modern DevOps environments

## Basic usage
- Start a tmux session:
```
tmux
```
- Detach from session:
```
Ctrl + b  d
```
- Reattach last session:
```
tmux attach
```

## Pane management
- Split vertically:
```
Ctrl + b  %
```
- Split horizontally:
```
Ctrl + b  "
```
- Switch between panes:
```
Ctrl + b  arrow keys
```

## Window management
- New window:
```
Ctrl + b  c
```
- Next window:
```
Ctrl + b  n
```
- Previous window:
```
Ctrl + b  p
```
- List windows:
```
Ctrl + b  w
```

## List tmux sessions
```
tmux ls
```

The `tmux` command
is widely used for
terminal session management
and long-running tasks.
