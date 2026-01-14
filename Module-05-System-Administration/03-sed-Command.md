# sed Command

The `sed` (Stream Editor) command is used
to perform basic text transformations
on input streams or files.

## Common uses
- Search and replace text
- Delete lines
- Print specific lines
- Edit files non-interactively

## Basic syntax
sed 'operation' file

## Common operations
- `s/old/new/` – substitute text
- `d` – delete lines
- `p` – print lines

## Examples
- `sed 's/root/admin/' file.txt` – replace first match
- `sed 's/root/admin/g' file.txt` – replace all matches
- `sed '/error/d' logfile` – delete lines containing "error"
- `sed -n '5,10p' file.txt` – print lines 5 to 10

The `sed` command is powerful
for automation and scripting tasks.
