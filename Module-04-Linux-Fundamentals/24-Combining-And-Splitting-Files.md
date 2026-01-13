# Combining and Splitting Files

Linux provides commands
to combine multiple files into one
or split large files into smaller parts.

## Combining files
- `cat file1 file2 > combined.txt` – merge files
- `cat *.txt > all_files.txt` – combine multiple files

## Splitting files
- `split -l 1000 file.txt part_` – split by number of lines
- `split -b 5M file.bin chunk_` – split by file size

## Examples
- `cat part_* > original_file`
- `split -b 10M backup.tar backup_part_`

Combining and splitting files
is useful for backups and file transfers.
