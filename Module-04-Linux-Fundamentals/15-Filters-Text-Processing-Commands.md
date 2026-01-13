# Filters and Text Processing Commands

Linux provides text processing commands
that filter, search, and manipulate output.

## Common filter commands
- `grep` – search text by pattern
- `sort` – sort lines of text
- `uniq` – remove duplicate lines
- `wc` – count lines, words, and characters
- `cut` – extract specific fields or columns
- `tr` – translate or delete characters

## Examples
- `grep error logfile`
- `sort names.txt`
- `uniq list.txt`
- `wc -l file.txt`
- `cut -d: -f1 /etc/passwd`

Text filters are powerful
when combined with pipes.
