# Truncate File Size (truncate)

The `truncate` command is used
to resize a file to a specified size
without editing its content.

## Common usage
- `truncate -s SIZE file` – set file to a specific size
- `truncate -s 0 file` – empty a file
- `truncate -s +1M file` – increase file size
- `truncate -s -1M file` – decrease file size

## Examples
- `truncate -s 0 logfile.log`
- `truncate -s 10M data.bin`

The `truncate` command is useful
for managing log files and disk usage.
