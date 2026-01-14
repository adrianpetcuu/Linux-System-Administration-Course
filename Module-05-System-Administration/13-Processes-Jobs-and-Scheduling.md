# Processes, Jobs, and Scheduling

Linux manages running programs
as processes and allows users
to control and schedule them.

## Processes
- A process is a running instance of a program
- Each process has a unique PID (Process ID)
- Common commands:
  - `ps` – display running processes
  - `top` / `htop` – real-time process monitoring
  - `kill` – send signals to processes

## Jobs
- Jobs are processes started from a shell
- Can run in foreground or background
- Common job control commands:
  - `&` – run a command in background
  - `jobs` – list current jobs
  - `fg` – bring job to foreground
  - `bg` – resume job in background
  - `Ctrl + Z` – suspend a running job

## Scheduling
- Scheduling controls when tasks run
- Two main schedulers:
  - `at` – schedule a one-time task
  - `cron` – schedule recurring tasks

## Examples
- `sleep 60 &`
- `crontab -e`
- `at 10:00`

Understanding processes, jobs,
and scheduling is essential
for Linux system administration.
