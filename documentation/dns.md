# DNS Configuration

## Objective
Verify name resolution in the Active Directory environment and create a custom host record.

## Implementation
- Used DNS integrated with the `abadi.local` domain.
- Created an A record named `server`.
- Assigned the record to `192.168.80.10`.

## Test
The Windows 11 domain client resolved:

`server.abadi.local -> 192.168.80.10`

The test was performed using `nslookup`.
