# Windows Server Supporting Lab

> Supporting infrastructure lab documenting Windows Server services that complement network engineering environments.

## Role in the Portfolio
This repository is a supporting lab rather than a separate career direction. Its purpose is to demonstrate Windows Server knowledge that can support networked enterprise environments, domain integration, DHCP/DNS services, access control, and endpoint connectivity.

## Lab Environment
- **Virtualization:** VMware
- **Server:** Windows Server 2025
- **Domain Controller:** DC01
- **Client:** Windows 11 Pro (PC-IT01)
- **Domain:** `abadi.local`
- **Server IP:** `192.168.80.10`
- **Default Gateway:** `192.168.80.2`

## Implemented Services

### Active Directory Domain Services
- Installed Active Directory Domain Services (AD DS).
- Created the `abadi.local` domain.
- Promoted DC01 to a Domain Controller.
- Created Organizational Units for departmental organization.
- Created domain users and security groups.

### Group Policy
- Created and tested Group Policy Objects.
- Applied a user policy for HR.
- Restricted Control Panel and PC settings access for HR users.
- Verified the policy from the domain client.

### DNS
- Used DNS integrated with Active Directory.
- Created and tested an A record:

`server.abadi.local -> 192.168.80.10`

- Verified name resolution from the Windows 11 client using `nslookup`.

### DHCP
- Installed the DHCP Server role.
- Created and activated a DHCP scope.
- Configured address distribution, exclusions, default gateway, and DNS settings.
- Tested automatic IP configuration from PC-IT01.

### Domain Client
- Configured Windows 11 Pro as a domain client.
- Joined PC-IT01 to `abadi.local`.
- Tested domain authentication and domain user sign-in.

### File Sharing and Permissions
- Created shared folders for departmental access.
- Configured Share Permissions and NTFS Permissions.
- Tested authorized and unauthorized access using different domain users.
- Applied restrictions so access could be controlled per department.

## Network Relevance
The lab demonstrates supporting services commonly encountered alongside enterprise networking, including:
- DNS and name resolution
- DHCP and IP address assignment
- Domain integration
- User and group administration
- Group Policy
- File sharing and access permissions
- Basic network troubleshooting

## Validation Tests
The following were tested successfully:
- Domain Controller connectivity
- Domain join
- Domain user sign-in
- Group Policy restrictions
- DNS name resolution with `nslookup`
- DHCP IP assignment
- Shared folder access
- NTFS permission restrictions

## Tools
- VMware
- Windows Server
- Windows 11 Pro

## Scope
This repository supports the primary Network Engineering portfolio. Advanced topics such as PKI, backup and recovery, multi-server environments, Microsoft Entra ID, Microsoft 365, and Azure integration are outside the current scope.

## Next Improvements
- Add screenshots from the actual lab.
- Add a simple network/lab topology diagram.
- Expand documentation with configuration and testing evidence.

---
Supporting Windows Server lab for a Network Engineering-focused portfolio.
