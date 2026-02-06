# Active Directory Structure

## OU Layout (as-built)

ApexTech
├── USERS
│   ├── Contractors
│   ├── Executives
│   ├── Finance
│   ├── HR
│   ├── IT
│   └── Sales
├── WORKSTATIONS
│   ├── FINANCE
│   ├── HR
│   ├── IT
│   ├── SALES
│   └── GENERAL
├── SERVERS
├── SERVICE_ACCOUNTS
└── GROUPS
    ├── Global
    └── DomainLocal

## OU Purpose Rules (no guessing)
For each OU: what belongs here, what should never be here, and why.

### OU: Corp\Users\Standard
- Contains: Normal user accounts
- Excludes: Admin and service accounts
- Why: Apply least-privilege user policies without affecting admins/services

### OU: Corp\Workstations\HR
- Contains: HR workstations
- Why: HR-specific GPOs (lockdown, mapped drives, printers, etc.)

## Groups & Admin Model (as-built)
- Domain Admins: [list which accounts are in it]
- Workstation local admin strategy: [explain]
- Service accounts strategy: [explain]
