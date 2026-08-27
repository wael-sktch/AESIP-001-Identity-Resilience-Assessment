# AESIP-001 Final Assessment Report

## Atlas Enterprise Security Improvement Program

### Executive Summary
AESIP-001 evaluated identity resilience from the perspective of a compromised standard employee workstation. The assessment focused on whether the attacker could discover infrastructure, access Active Directory services, reach the file server, and progress into sensitive departmental data.

An initial high-risk configuration issue was identified: the workstation was logged on using a Domain Administrator account, invalidating the original low-privilege attacker assumption and creating a potential Tier-0 credential exposure condition. A dedicated standard-user profile, `atlas.sarah`, was then used to establish the intended assessment scenario.

### Assessment Result
The standard user could discover authorized infrastructure and reach FS01, but access to Finance, HR, and IT departmental resources was denied. Public collaboration resources remained accessible as designed.

### Overall Rating
**82 / 100 — Moderately Mature**

| Area | Rating |
|---|---|
| Identity Security | Medium |
| Privileged Access | High Risk |
| File Access Controls | Low Risk |
| Active Directory Exposure | Low Risk |
| DNS Infrastructure | Low Risk |
| Kerberos Security | Low Risk |
| Attack Path Risk | Medium |

### Conclusion
The most significant risk discovered was privileged administrative exposure on a user workstation. After establishing the intended low-privilege scenario, authorization controls successfully prevented progression from FS01 into sensitive departmental data.

The principal improvement area is privileged access architecture: Tier-0 identities should be separated from daily-use activity and restricted to approved administrative systems.
