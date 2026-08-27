# Assessment Commands and Rationale

> Commands were executed only within the authorized Atlas lab environment.

| Command | Purpose |
|---|---|
| `whoami` | Identify the current account |
| `whoami /groups` | Review security group membership |
| `whoami /all` | Review full identity and privilege context |
| `nslookup FS01` | Validate DNS resolution |
| `Resolve-DnsName FS01` | Validate DNS records |
| `ping FS01` | Basic reachability validation |
| `Test-NetConnection FS01` | Connectivity validation |
| `net user /domain` | Enumerate domain users |
| `net group "Domain Admins" /domain` | Review Domain Admin membership |
| `net view \\DC01` | Enumerate visible shares |
| `dir \\DC01\SYSVOL` | Validate SYSVOL access |
| `klist` | Review Kerberos tickets |
| `gpresult /r` | Review applied Group Policy |
| `icacls \\FS01\Public` | Review Public share ACLs |
| `echo TEST > \\FS01\Public\file.txt` | Validate write access in Public share |
