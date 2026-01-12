# File Ownership Commands (chown, chgrp)

Linux files and directories
are owned by a user and a group.

## Ownership components
- User – file owner
- Group – group owner

## Changing file owner
- `chown user file`
- `chown user:group file`

## Changing group ownership
- `chgrp group file`

## Recursive ownership change
- `chown -R user:group directory`

Managing ownership is important
for controlling access and security.
