# Troubleshooting Log

## Issue: GPUpdate found in ADUC instead of GPMC
- **Symptom:** Couldn't find "Group Policy Update" option under 
  ADUC's right-click menu on an OU
- **Cause:** That feature lives in Group Policy Management Console 
  (GPMC), not ADUC — different tools, easy to mix up since both live 
  under Server Manager → Tools
- **Fix:** Opened GPMC instead, right-clicked OU → Group Policy Update

## Issue: "No computer objects found" when pushing GPO update to HR OU
- **Symptom:** GPMC reported no computers found in HR or sub-OUs
- **Cause:** Group Policy Update targets computer objects, not users — 
  and no client VM had been joined to the domain yet, so HR/Computers 
  was empty
- **Fix:** [update once client VM is joined and moved into the OU]
- **Takeaway:** GPO push is machine-based even for policies that 
  affect user experience (like login banners), which isn't obvious 
  until you hit it
