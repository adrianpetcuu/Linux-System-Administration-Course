# Talking to Users – users, wall, write

Linux provides commands
to communicate with users
logged into the system.

## users command
- Displays currently logged-in usernames
- Shows users in a simple format
- Example: `users`

## wall command
- Sends a message to all logged-in users
- Useful for system-wide announcements
- Example:
  - `echo "System maintenance in 10 minutes" | wall`

## write command
- Sends a message to a specific user
- Requires the user to be logged in
- Example:
  - `write john`
  - Type the message and press `Ctrl + D`

## Notes
- Users can block messages using `mesg n`
- Enable messages with `mesg y`

These commands are commonly used
by administrators for notifications
and user communication.
