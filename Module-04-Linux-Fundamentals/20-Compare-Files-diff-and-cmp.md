# Compare Files – diff and cmp

Linux provides commands
to compare the contents of files.

## diff command
- Shows line-by-line differences
- Commonly used for text files
- Useful for configuration comparisons

## cmp command
- Compares files byte by byte
- Reports the first difference found
- Commonly used for binary files

## Examples
- `diff file1.txt file2.txt`
- `diff -u file1.txt file2.txt`
- `cmp file1.bin file2.bin`

Use `diff` to see detailed changes
and `cmp` to check if files are identical.
