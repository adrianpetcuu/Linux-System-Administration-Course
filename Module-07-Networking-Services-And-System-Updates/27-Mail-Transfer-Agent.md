## Mail Transfer Agent (MTA)

A Mail Transfer Agent (MTA)
is responsible for sending,
receiving, and routing email
between mail servers.

### Common MTAs
- Postfix
- Sendmail
- Exim

### Role of an MTA
- Accepts outgoing mail from applications
- Routes mail to local or remote servers
- Delivers mail to local mailboxes or another MTA

### Postfix (Most Common)
- Secure and efficient
- Widely used on Linux systems
- Default MTA on RHEL/CentOS

### Basic Postfix Commands
```bash
systemctl start postfix
systemctl enable postfix
mailq
```

### Mail Logs
- `/var/log/maillog`

### Summary
An MTA is a core mail
infrastructure component
used to transfer emails
between systems reliably.
