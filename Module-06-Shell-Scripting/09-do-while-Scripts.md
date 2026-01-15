# do-while Scripts

The do-while loop executes
commands at least once
and repeats while a condition is true.

## do-while logic
- Commands run first
- Condition is checked after execution
- Implemented using `while` in shell scripting

## Syntax
```
do
  command
done
while [ condition ]
```

## Practical do-while example
```
#!/bin/bash
count=1
while true
do
  echo "Count: $count"
  count=$((count+1))
  if [ $count -gt 5 ]; then
    break
  fi
done
```

## Another example
```
#!/bin/bash
number=1
while [ $number -le 3 ]
do
  echo $number
  number=$((number+1))
done
```

do-while scripts
are useful when a task
must run at least once.
