# Findings Register

## F-001 — Domain Administrator on User Workstation

**Severity:** HIGH

### Evidence
`lab\administrator` was observed on `CLIENT`, a workstation located in the USERS VLAN.

### Risk
```text
Workstation compromise
        ↓
Privileged credential exposure
        ↓
Domain compromise
```

### Impact
A user endpoint should not routinely contain an active Tier-0 administrative session. Endpoint compromise under those conditions can materially increase the blast radius from a single workstation to the wider Active Directory environment.

### Remediation
- Separate daily-use and privileged administrative accounts.
- Use dedicated administrative workstations for Tier-0 administration.
- Restrict privileged account logon to approved systems.
- Review privileged group membership and interactive logon practices regularly.

### Status
Remediated for the assessment scenario by creating and using the dedicated standard-user profile `atlas.sarah`.
