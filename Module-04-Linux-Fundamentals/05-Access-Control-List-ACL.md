# Access Control List (ACL)

Access Control Lists (ACLs) provide
more flexible permission management
than standard Linux file permissions.

## Why use ACL
- Grant permissions to specific users or groups
- Extend access control beyond owner, group, and others
- Useful in shared environments

## Common ACL commands
- `getfacl file` – view ACL permissions
- `setfacl -m u:user:rwx file` – set ACL for a user
- `setfacl -m g:group:rw file` – set ACL for a group
- `setfacl -x u:user file` – remove ACL entry

## Default ACL
- `setfacl -d -m u:user:rwx directory`

ACLs are commonly used
when standard permissions are not sufficient.
