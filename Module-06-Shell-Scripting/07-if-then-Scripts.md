# if-then Scripts

The `if-then` statement allows
a shell script to make decisions
based on conditions.

## Basic if syntax
```
if [ condition ]; then
  command
fi
```

## if-else syntax
```
if [ condition ]; then
  command
else
  command
fi
```

## Numeric comparison
- `-eq` equal
- `-ne` not equal
- `-gt` greater than
- `-lt` less than

## String comparison
- `=` equal
- `!=` not equal
- `-z` string is empty

## Example script
```
#!/bin/bash
read number
if [ $number -gt 10 ]; then
  echo "Number is greater than 10"
else
  echo "Number is 10 or less"
fi
```

if-then scripts
are essential for logic
and automation in Linux.
