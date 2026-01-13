# awk – Text Processing Command

The `awk` command is a powerful
text processing tool used to manipulate
and analyze structured text.

## Basic usage
- `awk '{print $1}' file` – print first field
- Fields are separated by whitespace by default

## Common options
- `-F` – define a field separator
- `$0` – represents the entire line
- `$1, $2, ...` – represent individual fields

## Examples
- `awk '{print $1}' /etc/passwd`
- `awk -F: '{print $1}' /etc/passwd`
- `ls -l | awk '{print $9}'`

awk is widely used
for reporting and data extraction.
