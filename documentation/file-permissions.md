# File Sharing and Permissions

## Objective

Create department-based file access and validate authorization using domain accounts.

## Implementation

- Created shared departmental folders.
- Configured Share Permissions.
- Configured NTFS Permissions.
- Assigned access through appropriate domain users or security groups.
- Restricted unauthorized access to protected folders.

## Validation

Access was tested with different domain users.

The tests verified that:

- Authorized users could access their required folders.
- Restricted users could not access protected content.

## Key Concepts

The lab demonstrates the difference between Share Permissions and NTFS Permissions and how they can be combined to control access to network resources.

## Related Documentation

- Active Directory (active-directory.md)
- Group Policy Management (group-policy.md)
