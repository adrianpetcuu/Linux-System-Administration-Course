# cut – Text Processing Command

The `cut` command is used
to extract specific sections of text
from each line of a file or command output.

## Common options
- `-d` – specify a delimiter
- `-f` – select fields
- `-c` – select characters

## Examples
- `cut -d: -f1 /etc/passwd` – display usernames
- `cut -d, -f2 data.csv` – extract second column
- `cut -c1-5 file.txt` – extract first five characters

The `cut` command is commonly used
with pipes for text processing tasks.
