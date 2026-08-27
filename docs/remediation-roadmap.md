# Remediation Roadmap

## Immediate — Critical
### Remove routine administrative usage from user workstations
- Use dedicated administrative workstations.
- Separate standard and privileged identities.
- Restrict privileged interactive logons to approved administrative systems.

## Short-Term — High
### Implement tiered administration
- Tier 0: Domain and identity infrastructure
- Tier 1: Servers and applications
- Tier 2: User workstations

### Improve endpoint security baselines
Examples:
- PowerShell logging
- Windows Defender policies
- Appropriate removable-media controls

## Long-Term — Medium
### Active Directory Certificate Services assessment
Review:
- Certificate templates
- Enrollment rights
- Misconfiguration-driven attack paths
