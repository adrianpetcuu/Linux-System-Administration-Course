# Shell History

The shell history feature
stores previously executed commands
to improve efficiency and reuse.

## View command history
```
history
```

## Run commands from history
- `!!` – run last command
- `!n` – run command number n
- `!string` – run last command starting with string

## Search history
- Press `Ctrl + R`
- Type part of the command

## History files
- User history is stored in:
  - `~/.bash_history`

## History configuration variables
- `HISTSIZE` – number of commands kept in memory
- `HISTFILESIZE` – number of commands saved to file

## Clear history
```
history -c
```

Shell history
helps speed up command execution
and is essential for daily Linux usage.
