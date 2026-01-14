# SOS Report

An SOS Report is a diagnostic
tool used in Linux to collect
system configuration and
troubleshooting information.

## What is sosreport
- Collects system logs, configuration files,
  and command outputs
- Creates a compressed archive for analysis
- Commonly used in enterprise support cases
  (Red Hat, CentOS, Rocky Linux)

## Generate an SOS report
- Run as root:
- `sos report`
- Follow on-screen prompts
- The report is saved in `/var/tmp/`

## Example output file
- `/var/tmp/sosreport-hostname-date.tar.xz`

## What it includes
- System logs (`/var/log`)
- Hardware information
- Network configuration
- Running services and processes

## Notes
- Sensitive data may be included
- Review the report before sharing

SOS reports are essential
for advanced troubleshooting
and vendor support cases.
