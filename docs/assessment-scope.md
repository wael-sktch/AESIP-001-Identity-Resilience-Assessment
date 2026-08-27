# Assessment Scope

## Objective
Assess whether compromise of a standard employee workstation could provide access to, or a viable path toward, critical Atlas infrastructure and sensitive departmental data.

## Assumed Attacker Position
- User: `atlas.sarah`
- Host: `CLIENT`
- IP: `10.10.10.102`
- VLAN: USERS (`10.10.10.0/24`)
- Privilege: Standard Domain User

## Systems Reviewed
| System | Function |
|---|---|
| CLIENT | User workstation |
| DC01 | Active Directory, DNS, identity services |
| FS01 | Enterprise file services |
| PF01 | Firewall, routing, NAT, VLAN boundaries |
| WAZUH01 | Security monitoring |
| WAF01 | Web application firewall |
| WEB01 | Web application |

## Assessment Focus
- Identity security
- Domain exposure
- Authorization controls
- Attack path mapping
- Access validation
