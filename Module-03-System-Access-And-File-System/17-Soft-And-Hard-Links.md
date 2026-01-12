# Soft and Hard Links

Links in Linux are used to create references
to files within the file system.

## Hard links
- Point directly to the same inode as the original file
- Share the same data on disk
- Cannot cross file systems
- Remain valid if the original file is deleted

## Soft links (symbolic links)
- Point to the file path, not the inode
- Can cross file systems
- Become broken if the original file is removed
- Commonly used for shortcuts

## Creating links
- Hard link: ln file1 file2
- Soft link: ln -s file1 link1

Understanding links is important
for file management and system administration.
