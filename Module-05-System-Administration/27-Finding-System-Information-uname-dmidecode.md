# Finding System Information (uname, dmidecode)

Linux provides commands
to display kernel, hardware,
and system information.

## uname command
- Displays kernel and system details
- Common options:
  - `-a` – all system information
  - `-r` – kernel release
  - `-m` – machine hardware name

## Examples
- `uname`
- `uname -a`
- `uname -r`

## dmidecode command
- Displays hardware information from BIOS/DMI
- Requires root privileges
- Shows details about system, CPU, memory, and motherboard

## Examples
- `dmidecode`
- `dmidecode -t system`
- `dmidecode -t memory`
- `dmidecode -t processor`

These commands are useful
for identifying system hardware
and kernel details
during troubleshooting and audits.
