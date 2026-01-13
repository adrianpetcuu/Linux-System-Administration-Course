# Standard Output to a File (tee Command)

The `tee` command reads standard input
and writes it to both the terminal and a file.

## Basic usage
- `command | tee file.txt` – write output to file and display it
- `command | tee -a file.txt` – append output to a file

## Common use cases
- Save command output while viewing it
- Log results without hiding terminal output

## Example
- `ls -l | tee files.txt`

The `tee` command is useful
for monitoring and logging command output.
