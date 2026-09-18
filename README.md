# Windows Server Enterprise Lab

A hands-on Windows Server lab demonstrating enterprise infrastructure services that commonly support networked environments.

## Portfolio Role

This repository is a supporting infrastructure lab for a Network Engineering-focused portfolio.

It demonstrates practical knowledge of:

- Active Directory Domain Services
- DNS
- DHCP
- Group Policy
- Domain-joined Windows clients
- File sharing and permissions
- Basic enterprise network troubleshooting

## Lab Environment

| Component | Configuration |
|---|---|
| Hypervisor | VMware |
| Server | Windows Server 2025 |
| Domain Controller | DC01 |
| Client | Windows 11 Pro (PC-IT01) |
| Domain | abadi.local |
| Server IP | 192.168.80.10 |
| Default Gateway | 192.168.80.2 |

## Implemented Services

### Active Directory Domain Services
- Installed the AD DS role.
- Created the abadi.local domain.
- Promoted DC01 to a Domain Controller.
- Created Organizational Units.
- Created domain users and security groups.
- Joined the Windows 11 client to the domain.

### DNS
- Used Active Directory-integrated DNS.
- Created the A record server.abadi.local -> 192.168.80.10.
- Verified name resolution from the Windows 11 client with nslookup.

### DHCP
- Installed the DHCP Server role.
- Created and activated a DHCP scope.
- Configured the address range and exclusions.
- Configured the default gateway as 192.168.80.2.
- Configured DNS as 192.168.80.10.
- Verified automatic addressing from PC-IT01.

### Group Policy
- Created and configured Group Policy Objects.
- Applied an HR user policy.
- Restricted Control Panel and PC settings access for HR users.
- Verified the policy from the domain client.

### File Sharing & Permissions
- Created departmental shared folders.
- Configured Share Permissions.
- Configured NTFS Permissions.
- Tested authorized and unauthorized access with domain accounts.

## Validation

The following lab functions were tested:

- Domain Controller connectivity
- Domain join
- Domain user authentication
- DNS resolution with nslookup
- DHCP address assignment
- Group Policy restrictions
- Shared-folder access
- NTFS permission restrictions

## Network Relevance

This lab complements network engineering by demonstrating infrastructure services that directly affect client connectivity and enterprise operations:

DHCP -> IP addressing
DNS -> Name resolution
AD DS -> Identity and authentication
GPO -> Centralized endpoint policy
File permissions -> Controlled resource access

## Repository Structure

- README.md
- documentation/active-directory.md
- documentation/dhcp.md
- documentation/dns.md
- documentation/file-permissions.md
- documentation/group-policy.md

## Scope

Advanced topics such as PKI, backup and recovery, multi-server environments, Microsoft Entra ID, Microsoft 365, and Azure integration are outside the current lab scope.

## Next Improvements

- Add final lab screenshots.
- Add a simple lab topology diagram.
- Add command/configuration evidence.
- Expand testing documentation as the lab grows.

---

Portfolio focus: Windows Server • Active Directory • DNS • DHCP • Group Policy • File Permissions
