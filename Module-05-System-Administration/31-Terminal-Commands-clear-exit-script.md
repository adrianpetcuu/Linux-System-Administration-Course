# Terminal Commands – clear, exit, script

Linux provides basic terminal commands
to manage the screen, sessions,
and terminal activity recording.

## clear
- Clears the terminal screen
- Does not delete command history
- Example:
  - `clear`

## exit
- Closes the current shell session
- Logs out the current user
- Example:
  - `exit`

## script
- Records a terminal session
- Saves all input and output to a file
- Useful for audits and training

## Basic usage of script
- Start recording:
```
script session.log
```
- Stop recording:
```
exit
```

## Notes
- Default output file is `typescript`
- Requires no special permissions

These commands help manage
terminal sessions and
capture command activity.
