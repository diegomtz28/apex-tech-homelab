# Domain Purpose & Trust Model

## Domain
- Domain name: apextech.local
- Environment type: Single forest, single domain

## Purpose (what this lab is simulating)
This homelab simulates a small-to-mid enterprise Windows environment to practice:
- Identity and access management with Active Directory
- Centralized configuration using Group Policy
- Core infrastructure (DNS/DHCP/time)
- Automation and reliability engineering (health checks, drift detection, break/fix)

## Trust model (what trusts exist)
- Trusts: None (internal-only)
- Reason: Keep scope focused on internal identity control and reduce complexity.

## Critical services / “if this dies, everything suffers”
- DNS: DC01 hosts internal DNS
- Authentication: DC01 is the primary domain controller
- Time: Domain time authority is DC01 (Kerberos dependent)
