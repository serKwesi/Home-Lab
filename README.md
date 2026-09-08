# Home IT Support Lab — Active Directory & Group Policy

A self-built home lab simulating day-to-day Tier 1/2 IT support work: 
Active Directory administration, user lifecycle management, OU structure, 
and Group Policy — built entirely in VirtualBox to practice real helpdesk 
tasks in a safe, disposable environment.

## Why this project

This lab exists to practice the actual daily task of IT support: resetting passwords, 
managing locked accounts, organizing users into departments, and pushing 
policies that affect real (virtual) machines — then troubleshooting when 
they don't behave as expected.

## Environment

| Component        | Details                                |
|-------------------|-----------------------------------------|
| Hypervisor         | VirtualBox                              |
| Domain Controller  | Windows Server (AD DS, DNS)             |
| Domain             | cloudlab.local                          |
| Client             | Windows 10                              |
| Networking         | Bridged Adapter (VMs on home LAN, visible to router) |

## What this demonstrates

- Installing and configuring Active Directory Domain Services
- Creating and managing user accounts (reset, disable, enable, unlock)
- Designing an OU structure for a multi-department organization
- Creating and scoping Group Policy Objects (login banners, password 
  policy, software restriction)
- Joining a client machine to a domain and troubleshooting connectivity
- Verifying policy application end-to-end via `gpupdate` and remote 
  GPO push

## Structure

- `01-vm-setup.md` — VirtualBox configuration and networking
- `02-active-directory.md` — Domain controller setup
- `03-users-ous.md` — User accounts and OU design
- `04-group-policy.md` — GPOs created, their purpose, and scope
- `05-troubleshooting-log.md` — Real issues hit and how they were resolved
- `screenshots/` — Supporting screenshots for each stage

cloudlab.local
├── IT-Department → IT-Admins group
├── HR → HR-Team group
├── Engineering → Engineering-Team group
└── Finance → Finance-Team group


## Scenarios Practiced

- Password reset
- Account lockout and unlock
- New user onboarding
- User offboarding
- GPO troubleshooting
- Remote desktop support

## Author

Kwasi Serebuor
[LinkedIn](https://www.linkedin.com/in/Kwasi-Serebuor) 
[GitHub](https://github.com/serKwesi)
