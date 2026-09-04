# Group Policy Objects

## GPO 1 — Login Banner
- **Setting:** Interactive logon message text/title
- **Linked to:** IT OU
- **Purpose:** Simulates a compliance/legal notice at login
- **Verified:** Logged in as IT user → banner appeared. Logged in as 
  user from another OU → banner did not appear (confirms scoping).

## GPO 2 — Password Policy
- **Setting:** [fill in exact settings you changed]
- **Linked to:** [OU]
- **Purpose:** Enforce complexity/length/expiry rules
- **Verified:** [how you tested it]

## GPO 3 — Restrict Software Installation
- **Setting:** [fill in]
- **Linked to:** [OU]
- **Purpose:** Prevent standard users installing unauthorized software
- **Verified:** [how you tested it]

## Group Policy Update
- Pushed remotely via GPMC → right-click OU → Group Policy Update
- Alternative/local method: `gpupdate /force` on the target machine
