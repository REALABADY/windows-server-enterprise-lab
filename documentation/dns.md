# DNS Configuration

## Objective

Provide and validate name resolution in the Active Directory environment.

## Implementation

- Used DNS integrated with the abadi.local domain.
- Created an A record named server.
- Assigned the record to 192.168.80.10.

## Record

server.abadi.local -> 192.168.80.10

## Validation

The Windows 11 domain client resolved the server name successfully using:

nslookup server.abadi.local

## Network Relationship

DNS is essential for Active Directory because domain services rely on reliable name resolution.

## Related Documentation

- Active Directory (active-directory.md)
- DHCP Configuration (dhcp.md)
