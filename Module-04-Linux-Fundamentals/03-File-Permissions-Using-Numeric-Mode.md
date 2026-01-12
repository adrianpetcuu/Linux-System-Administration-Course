# File Permissions Using Numeric Mode

Linux permissions can be set
using numeric (octal) values.

## Numeric values
- 4 – read (r)
- 2 – write (w)
- 1 – execute (x)

## Permission calculation
- 7 = rwx (4+2+1)
- 6 = rw- (4+2)
- 5 = r-x (4+1)
- 4 = r-- (4)

## Example
- `chmod 755 script.sh` – rwx for owner, r-x for group and others

Numeric mode provides a quick
and precise way to manage permissions.
