# Compress and Uncompress (tar, gzip, gunzip)

Linux provides tools
to archive and compress files
for storage and transfer.

## tar command
- Used to create and extract archives
- Common options:
  - `-c` – create archive
  - `-x` – extract archive
  - `-v` – verbose output
  - `-f` – specify archive file

## gzip and gunzip
- `gzip` – compress files
- `gunzip` – decompress files

## Examples
- `tar -cvf archive.tar directory/`
- `tar -xvf archive.tar`
- `tar -czvf archive.tar.gz directory/`
- `tar -xzvf archive.tar.gz`
- `gzip file.txt`
- `gunzip file.txt.gz`

These tools are essential
for backup and file distribution.
