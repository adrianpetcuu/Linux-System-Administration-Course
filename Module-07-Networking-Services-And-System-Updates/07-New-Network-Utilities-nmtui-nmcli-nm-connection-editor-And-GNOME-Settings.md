## New Network Utilities

Modern Linux systems use **NetworkManager**
and its tools to configure and manage
network connections.

### nmtui
- Text-based (TUI) network configuration tool
- Easy to use in terminal environments
- Useful when GUI is not available

```bash
nmtui
```

---

### nmcli
- Command-line tool for NetworkManager
- Script-friendly and powerful
- Preferred for automation and exams

```bash
nmcli device status
nmcli connection show
nmcli connection up enp0s3
nmcli device disconnect enp0s8
```

---

### nm-connection-editor
- Graphical network configuration tool
- Allows detailed editing of connections
- Requires a graphical environment

```bash
nm-connection-editor
```

---

### GNOME Settings
- GUI-based network management
- Used mainly on desktop systems
- Located at: Settings → Network

---

### Summary
NetworkManager utilities provide
multiple ways to manage network
connections depending on the system
and environment.
