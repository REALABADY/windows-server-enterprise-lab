# Windows Server Enterprise Lab

## Overview
A hands-on Windows Server lab designed to simulate a small enterprise environment. The lab focuses on core infrastructure services, domain administration, network services, endpoint integration, and access control.

## Lab Environment
- **Virtualization:** VMware
- **Server:** Windows Server 2025
- **Domain Controller:** DC01
- **Client:** Windows 11 Pro (PC-IT01)
- **Domain:** `abadi.local`
- **Server IP:** `192.168.80.10`
- **Default Gateway:** `192.168.80.2`

## Implemented Technologies

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

## Skills Demonstrated
- Windows Server Administration
- Active Directory Domain Services
- User and Group Management
- Organizational Units
- Group Policy Management
- DNS Administration
- DHCP Configuration
- Domain Integration
- File Sharing
- NTFS and Share Permissions
- Basic Network Troubleshooting
- VMware Virtualization

## Project Status
Core Windows Server administration services have been implemented and tested. Advanced topics such as PKI, backup and recovery, multi-server environments, Microsoft Entra ID, Microsoft 365, and Azure integration are intentionally outside the current scope.

## Repository Structure
```text
windows-server-enterprise-lab/
├── README.md
├── documentation/
│   ├── active-directory.md
│   ├── dns.md
│   ├── dhcp.md
│   ├── group-policy.md
│   └── file-permissions.md
└── screenshots/
```

## Next Improvements
- Add screenshots from the actual lab.
- Add a simple network/lab topology diagram.
- Expand documentation with configuration and testing evidence.

---
Built as a hands-on IT Infrastructure and Windows Server administration lab.
