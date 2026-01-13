# Executing Multiple Commands

Linux allows multiple commands
to be executed in a single line.

## Command separators
- `;` – run commands sequentially
- `&&` – run next command only if the previous succeeds
- `||` – run next command only if the previous fails

## Examples
- `cmd1; cmd2`
- `cmd1 && cmd2`
- `cmd1 || cmd2`

Executing multiple commands
improves efficiency and scripting flexibility.
