# Basic Shell Scripting

Basic shell scripting allows
automation of simple tasks
using Linux shell commands.

## Script structure
- Start with a shebang:
```
#!/bin/bash
```
- Commands are executed line by line

## Variables
- Define a variable:
```
name="Linux"
```
- Use a variable:
```
echo $name
```

## User input
```
read username
echo "Hello $username"
```

## Conditional statement
```
if [ $value -gt 10 ]; then
  echo "Value is greater than 10"
fi
```

## Loop example
```
for i in 1 2 3
do
  echo $i
done
```

Basic shell scripting
is the foundation for
Linux automation and RHCSA.
