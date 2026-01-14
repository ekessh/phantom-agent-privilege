# Phantom Privilege Ratio

## Definition
Percentage of active machine identities or credentials without verifiable human or workflow attribution.

## Formula
(Unattributed machine identities / Total active machine identities) × 100

## Target
- Production target: below 10%
- Regulated or high-impact paths: below 1% is preferred where feasible

## Practical notes
- "Unattributed" means missing at least one of: creator, originating workflow, purpose, or expiry.
- Track monthly, and after any agent capability or workflow changes.
