# Input and Output Redirection

Linux allows redirecting input and output
between commands and files.

## Standard streams
- stdin (0)  – standard input
- stdout (1) – standard output
- stderr (2) – standard error

## Output redirection
- `>`  – redirect stdout (overwrite)
- `>>` – redirect stdout (append)
- Example: `ls > files.txt`

## Input redirection
- `<` – redirect input from a file
- Example: `sort < names.txt`

## Error redirection
- `2>`  – redirect stderr
- `&>`  – redirect stdout and stderr
- Example: `command &> output.log`

Redirection is essential
for automation and scripting.
