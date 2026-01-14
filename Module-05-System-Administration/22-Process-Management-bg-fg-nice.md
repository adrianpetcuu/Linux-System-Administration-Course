# Process Management – bg, fg, nice

Linux provides commands
to control running processes
and manage their priority.

## bg command
- Resumes a suspended job in the background
- Job continues running without blocking the terminal
- Example:
  - `bg %1`

## fg command
- Brings a background or suspended job
  to the foreground
- Example:
  - `fg %1`

## nice command
- Starts a process with a defined priority
- Priority range: -20 (highest) to 19 (lowest)
- Default priority is 0

## Examples
- Run a command with lower priority:
- `nice -n 10 command`
- Check process priority:
- `ps -o pid,ni,cmd`

Process management commands
help control system performance
and are commonly tested in RHCSA.