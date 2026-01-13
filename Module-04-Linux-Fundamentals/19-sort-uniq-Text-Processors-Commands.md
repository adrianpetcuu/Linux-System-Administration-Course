# sort and uniq – Text Processing Commands

The `sort` and `uniq` commands are used
to organize and filter text output.

## sort command
- Sorts lines alphabetically or numerically
- Common options:
  - `-n` – numeric sort
  - `-r` – reverse order
  - `-k` – sort by a specific field

## uniq command
- Filters out duplicate adjacent lines
- Common options:
  - `-c` – count occurrences
  - `-d` – show duplicate lines only
  - `-u` – show unique lines only

## Examples
- `sort names.txt`
- `sort -n numbers.txt`
- `sort file.txt | uniq`
- `sort file.txt | uniq -c`

The `uniq` command is typically used
together with `sort` for accurate results.
