# Azure Conditional Access & Privileged Identity Design Program

This repository contains an enterprise-style Identity and Access Management design focused on Azure Conditional Access and privileged identity governance.

## Objectives
- Enforce strong access controls for standard users and tiered administrators
- Separate standard identities from privileged admin identities
- Block legacy authentication across the tenant
- Preserve emergency access using break-glass accounts with compensating controls
- Define privileged identity lifecycle governance: creation, assignment, expiration, review, and decommission
- Document validation expectations, failure scenarios, and incident triggers

## Identity Model
- Standard users
- Privileged administrators (Tier 0, Tier 1, Tier 2)
- Break-glass administrators (excluded from Conditional Access by design, governed operationally)

## Repo Layout
- docs: program documentation and policy blueprints
- blueprints: CSV inventories for policy tracking and tier mapping
- evidence: screenshots and proof artifacts once implemented
- diagrams: simple diagrams and legends (optional)
