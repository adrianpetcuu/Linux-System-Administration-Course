# kill Command

The `kill` command is used
to send signals to processes
to control or terminate them.

## Common signals
- `SIGTERM (15)` – gracefully stop a process
- `SIGKILL (9)` – forcefully terminate a process
- `SIGHUP (1)` – reload process configuration

## Basic usage
- `kill PID`
- `kill -9 PID`
- `kill -15 PID`

## Examples
- `kill 1234`
- `kill -9 1234`
- `kill -HUP 1234`

The `kill` command
is essential for managing
unresponsive or misbehaving processes.
