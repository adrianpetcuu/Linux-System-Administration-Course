# case Statement Scripts

The `case` statement allows
a shell script to execute
different actions based on
a matching pattern.

## Basic case syntax
```
case variable in
  pattern1)
    command
    ;;
  pattern2)
    command
    ;;
  *)
    default command
    ;;
esac
```

## Example script
```
#!/bin/bash
read choice

case $choice in
  start)
    echo "Starting service"
    ;;
  stop)
    echo "Stopping service"
    ;;
  restart)
    echo "Restarting service"
    ;;
  *)
    echo "Invalid option"
    ;;
esac
```

## Notes
- Each case ends with `;;`
- `*` is the default case
- Easier than multiple if-else blocks

The `case` statement
is useful for menus,
options, and automation scripts.
