# Lab Inventory

## Network
- Subnet(s): [10.10.1.0/24]
- Default gateway: [10.10.1.1]
- DNS server(s): [10.10.1.150]

## Hosts (VMs)
| Name | OS | IP | Role |
|------|----|----|------|
| DC01 | Windows Server 2022 | 10.10.1.150| AD DS, DNS, time authority |
| FS01 | Windows Server 2022 | 10.10.1.110 | File server |
| pfSense | FreeBSD | 10.10.1.1| Firewall, routing, NAT, network security |
| WS01 | Windows 11 | 10.10.1.100 | Domain-joined client |
| HD01 | Windows Server 2022 | 10.10.1.200 | Helpdesk/ticket system |

## Notes
