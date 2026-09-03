# DHCP Server Configuration

## Objective
Provide automatic network configuration to the Windows 11 domain client.

## Implementation
- Installed the DHCP Server role.
- Created and activated a DHCP scope.
- Configured the address range.
- Added an exclusion for the server's static IP.
- Configured the default gateway as `192.168.80.2`.
- Configured DNS to use `192.168.80.10`.

## Validation
PC-IT01 was configured to obtain network settings automatically and successfully received an IP address and network configuration from DHCP.
