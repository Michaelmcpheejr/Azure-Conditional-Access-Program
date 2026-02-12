# Conditional Access Policy Blueprints

## Policy Set Overview
This program defines the following Conditional Access policy types:
- User baseline policy
- User exception policies
- Admin tier policies (Tier 0, Tier 1, Tier 2)
- Dedicated legacy authentication block policy
- Global break-glass exclusion (operationally governed)

## Baseline User Policy
Name: CA-Users-Baseline-MFA
Applies to: Standard users
Intent: Require MFA for standard users for cloud access
Exclusions: None by default (exceptions handled separately)

## User Exception Policies
Name: CA-Users-Exception-<Reason>
Applies to: Standard users with documented exception
Intent: Explicitly manage any exception case without weakening baseline
Notes: Exceptions must be time-bound and reviewed

## Tier 0 Admin Policy
Name: CA-Admins-Tier0-StrongAuth
Applies to: Tier 0 admin identities
Intent: Strongest admin authentication requirements

## Tier 1 Admin Policy
Name: CA-Admins-Tier1-StrongAuth
Applies to: Tier 1 admin identities
Intent: Strong authentication requirements, slightly less restrictive than Tier 0

## Tier 2 Admin Policy
Name: CA-Admins-Tier2-StrongAuth
Applies to: Tier 2 admin identities
Intent: Strong authentication requirements appropriate for workstation scoped admin duties

## Legacy Authentication Block Policy
Name: CA-Block-LegacyAuth-All
Applies to: All identities (standard and admin)
Intent: Block legacy authentication to prevent MFA bypass
