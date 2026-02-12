# Validation and Failure Scenarios

## Validation Approach
Conceptual validation plus targeted testing.

## Acceptable Failures
- MFA failure denies access
- Admin denied access if requirements not met
- Break-glass bypasses CA by design
- Misconfiguration may temporarily block access (must be recoverable)

## Unacceptable Failures
- Standard user gains admin access
- Admin accesses Tier 0 without Tier 0 identity
- Legacy authentication succeeds
- Break-glass used without alerting

## What Success Looks Like
- Users and admins are enforced according to identity class and tier
- Legacy authentication is blocked tenant-wide
- Break-glass remains usable and is governed
- Policy changes are controlled and reviewable
