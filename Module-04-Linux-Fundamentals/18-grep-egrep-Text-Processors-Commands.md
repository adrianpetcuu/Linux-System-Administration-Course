# grep and egrep – Text Processing Commands

The `grep` and `egrep` commands are used
to search for patterns inside text files
or command output.

## grep command
- Searches for basic patterns
- Supports regular expressions
- Example: `grep root /etc/passwd`

## egrep command
- Supports extended regular expressions
- Equivalent to `grep -E`
- Example: `egrep "root|user" /etc/passwd`

## Common options
- `-i` – ignore case
- `-v` – invert match
- `-n` – show line numbers
- `-r` – recursive search

## Examples
- `grep error logfile`
- `grep -i ssh /var/log/messages`
- `grep -v root /etc/passwd`
- `egrep "http|https" access.log`

grep and egrep are essential tools
for searching and filtering text in Linux.
