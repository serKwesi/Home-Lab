# Active Directory Setup

## Steps taken
1. Installed AD DS role via Server Manager
2. Promoted server to domain controller
3. Created new forest: `cloudlab.local`
4. Verified via DNS and `Get-ADDomain` (or ADUC opening successfully)

## Why this matters
Every downstream task (users, OUs, GPOs) depends on this being correct — 
DNS in particular is the most common source of "client can't find the 
domain" issues later.
