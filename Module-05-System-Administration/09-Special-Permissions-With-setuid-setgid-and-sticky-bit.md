# Special Permissions – setuid, setgid, and Sticky Bit

Linux provides special permissions
that control how files and directories
behave beyond standard read, write,
and execute permissions.

## setuid (Set User ID)
- Executable runs with the file owner's privileges
- Commonly used by system binaries
- Example:
  - `chmod u+s file`
- Appears as `s` in the user execute field

## setgid (Set Group ID)
- Executable runs with the file group’s privileges
- On directories, new files inherit the group
- Example:
  - `chmod g+s directory`
- Appears as `s` in the group execute field

## Sticky Bit
- Used on directories
- Only the file owner or root can delete files
- Commonly applied to `/tmp`
- Example:
  - `chmod +t directory`
- Appears as `t` in the others execute field

## Numeric values
- setuid = 4
- setgid = 2
- sticky bit = 1
- Example:
  - `chmod 4755 file`

Special permissions
are important for security
and shared directories.
