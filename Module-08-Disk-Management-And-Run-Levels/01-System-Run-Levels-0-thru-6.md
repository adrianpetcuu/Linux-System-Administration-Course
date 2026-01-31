## System Run Levels (0–6)

Linux run levels define the **state of the system** and which services are running.
(Traditional SysV init concept; still important for understanding Linux fundamentals.)

### Run Levels Overview

- **0 – Halt**
  - Shuts down the system
  - Power off
  - Equivalent to: `shutdown -h now`

- **1 – Single User Mode**
  - Maintenance mode
  - No networking
  - Used for system recovery or repairs

- **2 – Multi-User (No Network)**
  - Multiple users
  - Limited services
  - Rarely used on modern systems

- **3 – Multi-User (CLI)**
  - Full multi-user mode
  - Networking enabled
  - No graphical interface
  - Common on servers

- **4 – Undefined / Custom**
  - Not used by default
  - Can be customized by administrators

- **5 – Multi-User with GUI**
  - Full system with graphical interface
  - Default for desktop systems

- **6 – Reboot**
  - Restarts the system
  - Equivalent to: `reboot`

### Modern Systems (systemd)
Modern Linux uses **systemd targets** instead of run levels:
- Runlevel 3 → `multi-user.target`
- Runlevel 5 → `graphical.target`

### Useful Commands
```bash
runlevel
systemctl get-default
systemctl isolate multi-user.target
systemctl isolate graphical.target
```

### Summary
- Run levels control system behavior
- Servers usually run at **3**
- Desktops usually run at **5**
- **0 = shutdown**, **6 = reboot**
