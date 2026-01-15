# Input and Output of a Script

Shell scripts can receive input
from users or files and produce output
to the terminal or files.

## Script input
- Read input from user:
```
read name
echo "Hello $name"
```

- Read arguments:
```
echo "Script name: $0"
echo "First argument: $1"
```

## Script output
- Standard output (stdout):
```
echo "Message"
```

- Redirect output to file:
```
echo "Hello" > output.txt
```

- Append output to file:
```
echo "Hello again" >> output.txt
```

## Error output
- Redirect errors:
```
command 2> error.log
```

## Example script
```
#!/bin/bash
read value
echo "You entered: $value"
```

Understanding script input and output
is essential for automation
and shell scripting.
