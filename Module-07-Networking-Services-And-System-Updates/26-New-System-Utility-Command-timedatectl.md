## timedatectl Command

The `timedatectl` command
is used to manage system
date, time, and time zone
on Linux systems.

### Display Current Time Settings
```bash
timedatectl
```

### Set Time Zone
```bash
timedatectl list-timezones
timedatectl set-timezone Europe/Bucharest
```

### Enable or Disable NTP
```bash
timedatectl set-ntp true
timedatectl set-ntp false
```

### Set Date and Time Manually
```bash
timedatectl set-time "2026-01-01 12:00:00"
```

### Check Hardware Clock Sync
- Shows if RTC is synchronized
- Works with `chronyd`

### Summary
`timedatectl` provides a simple
way to manage system time,
time zones, and NTP settings
on modern Linux systems.
