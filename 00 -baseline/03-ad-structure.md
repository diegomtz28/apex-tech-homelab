# Active Directory Structure

## OU Layout (as-built)

- apextech.local
    - USERS
        - Contractor
        - Executives
        - Finance
        - HR
        - IT
        -  Sales
- WORKSTATIONS
  - FINANCE
  - HR
  - IT
  - SALES
  - GENERAL
- SERVERS
- SERVICE_ACCOUNTS
-  GROUPS
    - Global
    - DomainLocal

## OU Purpose Rules (no guessing)
For each OU: what belongs here, what should never be here, and why.

### OU: Contains: Human user accounts only
- Contains: Normal user accounts
- Excludes: Computer objects, service accounts
- Why: Allows user-focused GPOs without impacting machines or services

### OU: Corp\Workstations\HR
- Contains: HR workstations
- Why: HR-specific GPOs (lockdown, mapped drives, printers, etc.)

## Groups & Admin Model (as-built)
- Domain Admins: [list which accounts are in it]
- Workstation local admin strategy: [explain]
- Service accounts strategy: [explain]
