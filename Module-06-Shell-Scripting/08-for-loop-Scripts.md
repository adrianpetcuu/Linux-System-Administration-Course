# for Loop Scripts

The `for` loop is used
to execute commands repeatedly
for a list of values.

## Basic for loop syntax
```
for variable in list
do
  command
done
```

## Example with numbers
```
#!/bin/bash
for i in 1 2 3 4 5
do
  echo "Number: $i"
done
```

## Example with files
```
for file in *.txt
do
  echo $file
done
```

## C-style for loop
```
for (( i=1; i<=5; i++ ))
do
  echo $i
done
```

for loops
are commonly used
in automation
and shell scripting.
