# Aliases

Aliases allow you
to create shortcuts
for longer or frequently
used Linux commands.

## What is an alias
- A custom name for a command
- Used to save time and reduce typing
- Works only in the shell where it is defined

## Create an alias
```
alias ll='ls -l'
```

## View aliases
```
alias
```

## Remove an alias
```
unalias ll
```

## Make aliases permanent
- Add aliases to:
  - `~/.bashrc`
  - `~/.bash_aliases` (if supported)

## Example
```
alias rm='rm -i'
```

Aliases are commonly used
to improve productivity
and avoid mistakes.
