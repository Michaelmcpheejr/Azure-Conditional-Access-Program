# Identity Model

## Identity Classes
1. Standard Users
2. Privileged Administrators
3. Break-Glass Administrators

## Privileged Identity Separation
Privileged access uses separate admin accounts. Standard and admin identities are not combined.

## Admin Tiering
Tiered model aligned to on-prem concepts:
- Tier 0: highest privilege (tenant-wide identity control plane)
- Tier 1: infrastructure and high-impact admin roles
- Tier 2: workstation and operator-level roles

## Trust Boundary Philosophy
Layered trust is used. Access decisions incorporate multiple signals where available.

## Exclusions Strategy
Exclusions are handled via separate policies and explicit governance, not hidden inside baseline enforcement.
