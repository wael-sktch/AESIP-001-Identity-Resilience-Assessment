# Attack Path Analysis

## Initial Access
**Identity:** `atlas.sarah`  
**Level:** Standard Domain User

## Discovery
The assessment validated discovery of:
- DC01
- FS01
- Domain Users
- Domain Admins
- SYSVOL
- NETLOGON

## Lateral Movement Validation
**Target:** FS01  
**Result:** Reachable; authorization boundary encountered.

## Data Access Results
| Resource | Result |
|---|---|
| Finance | ❌ Denied |
| HR | ❌ Denied |
| IT | ❌ Denied |
| Public | ✅ Allowed |

## Final Validated Path
```text
atlas.sarah
      ↓
CLIENT
      ↓
FS01
      ↓
Authorization Controls
      ↓
Sensitive Departmental Data Protected
```

The standard-user attack path did not progress into unauthorized departmental data.
