# Privileged Identity Lifecycle

## Admin Account Creation
Admin accounts are created only upon approved access request.

## Naming Standard
Admin tier embedded in username for quick identification during incidents.
Example patterns:
- <user>-t0adm
- <user>-t1adm
- <user>-t2adm

## Privilege Assignment
Privileges are granted through RBAC security group membership. Avoid direct role sprawl.

## Duration Model
Privileged access is time-bound with expiration by design intent. If tooling cannot enforce automatically, expiration is tracked operationally.

## Review Cadence
Privileged access reviews occur monthly.

## Decommission
When privileged access is no longer required:
- remove RBAC group membership
- disable admin account if no longer needed
- retain records for audit
