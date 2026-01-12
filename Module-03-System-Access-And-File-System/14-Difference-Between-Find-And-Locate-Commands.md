# Difference Between Find and Locate Commands

The `find` and `locate` commands are used to search for files
and directories, but they work differently.

## find command
- Searches the file system in real time
- Always shows current results
- Slower, but more accurate
- Example: find /home -name file.txt

## locate command
- Searches a prebuilt database
- Very fast
- Results may be outdated
- Example: locate file.txt

Use `find` for accuracy and advanced filters,
and `locate` for quick searches.
