# DHCP Server Configuration

## Objective

Provide automatic network configuration to the Windows 11 domain client.

## Implementation

1. Installed the DHCP Server role.
2. Created and activated a DHCP scope.
3. Configured the address range.
4. Added an exclusion for the server's static IP.
5. Configured the default gateway as 192.168.80.2.
6. Configured DNS as 192.168.80.10.

## Validation

PC-IT01 was configured to obtain network settings automatically and successfully received an IP address and network configuration from DHCP.

## Network Relationship

DHCP provides the client with the addressing information required to communicate with the local network and reach the DNS service.

## Related Documentation

- DNS Configuration (dns.md)
- Active Directory (active-directory.md)
