# Difference Between Active Directory, LDAP, IDM, Winbind, and OpenLDAP

Linux can integrate with different
directory and authentication technologies,
each serving a specific role.

## Active Directory (AD)
- Microsoft directory service
- Uses LDAP, Kerberos, and DNS
- Centralized user, group, and policy management
- Common in Windows-based environments

## LDAP
- Protocol used for directory access
- Defines how clients query directory servers
- Used by many services, including AD and OpenLDAP
- Not a directory service by itself

## IDM (Identity Management / FreeIPA)
- Linux-native identity management solution
- Combines LDAP, Kerberos, DNS, and certificates
- Centralized authentication for Linux systems
- Alternative to Active Directory in Linux environments

## OpenLDAP
- Open-source LDAP directory server
- Provides LDAP-based authentication
- Lightweight and flexible
- Lacks built-in policy and Kerberos integration by default

## Winbind
- Service used to integrate Linux with Active Directory
- Allows AD users to authenticate on Linux
- Maps Windows users and groups to Linux accounts
- Commonly used with Samba

## Summary
- Active Directory: full Windows identity solution
- LDAP: directory access protocol
- IDM/FreeIPA: enterprise Linux identity management
- OpenLDAP: basic LDAP directory server
- Winbind: bridge between Linux and Active Directory

Understanding these differences
is important for enterprise
Linux authentication design.
