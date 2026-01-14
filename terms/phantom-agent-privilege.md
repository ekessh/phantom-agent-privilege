# Phantom Agent Privilege
Version: v1.0

## Definition
Phantom agent privilege occurs when autonomous AI agents or automated workflows create, modify, or extend access credentials, service accounts, or permissions without durable human attribution or explicit approval records. Unlike orphaned or stale service accounts, these privileges are actively generated and exercised by autonomous systems, creating hidden escalation paths that can be exploited while appearing indistinguishable from legitimate activity.

## How teams recognize it
- Security alerts flag activity from valid but unexplained machine identities, with creation traced to agent-generated actions rather than named human approvers.
- Incident response stalls at "Who approved this access?", with answers pointing to automation workflows instead of accountable roles.
- Identity inventories show rapid growth in non-human identities that exceeds documented processes or expected workload changes.

## Indicators and thresholds
- More than 20% of active credentials lack creation metadata such as creator agent ID, originating workflow, purpose tag, or expiry.
- Autonomous workflows can provision permissions beyond read-only access without mandatory human review or approval checkpoints.
- Privilege sprawl velocity exceeds 50% quarterly growth in machine identities without a corresponding increase in access tickets or change requests.

## Mitigation reference
- Enforce privilege tagging so every agent-generated identity or permission logs creator, purpose, scope, and expiry, with default auto-revocation such as 72 hours.
- Implement attribution chains linking agent-spawned credentials to parent workflows using immutable metadata that survives rotation and reuse.
- Baseline expected privilege scopes and alert on abnormal expansions beyond approved agent permission patterns.

## Measurement hook
**Phantom Privilege Ratio**  
Percentage of active machine identities or credentials without verifiable human or workflow attribution.  
Target: below 10% for production environments.

## Derived from real incidents
Derived from recurring patterns observed in non-human identity compromise, automated credential misuse in supply-chain incidents, and over-privileged agent deployments described in public security reporting and incident analysis.

## Notes
This term describes a failure pattern independent of vendor, cloud provider, or identity platform.
