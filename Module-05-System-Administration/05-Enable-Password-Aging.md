# Enable Password Aging

Password aging enforces rules
that control how long a password
remains valid in Linux.

## Why password aging
- Improves system security
- Forces regular password changes
- Prevents long-term password reuse

## Enable password aging
- Use the `chage` command

## Common options
- `-m` – minimum days before password change
- `-M` – maximum password age
- `-W` – warning days before expiration
- `-I` – inactive days after expiration

## Example
- `chage -m 5 -M 90 -W 7 -I 3 username`

Password aging settings
are stored in `/etc/shadow`
and are commonly tested in RHCSA.
