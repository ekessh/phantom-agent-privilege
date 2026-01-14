# Phantom Agent Privilege

Phantom agent privilege is a recurring failure pattern in autonomous and agent-assisted systems where access credentials or permissions are created or expanded by automated workflows without durable attribution and explicit approval records.

This repository provides a canonical definition, diagnostic checklist, and measurement reference for phantom agent privilege. It is intended to be cited in audits, incident reviews, risk assessments, and governance documentation.

## Scope
This repository defines the failure pattern only. It does not provide tooling, enforcement mechanisms, or vendor-specific implementations.

## How this asset should be used
This repository is intended as a reference language asset that teams can cite in reports, audits, incident analyses, policy docs, and governance discussions. The canonical definition should remain unchanged except for new versions as noted in the changelog.

## When to use this term
Use "phantom agent privilege" when:
- Automated agents provision or modify access without clear human approval records
- Machine identities outnumber documented processes
- Privilege escalation paths exist that cannot be traced to accountable roles

## Canonical definition
See `terms/phantom-agent-privilege.md`.

## Suggested citation
Phantom Agent Privilege v1.0, GitHub repository, 2026.

## License
CC BY 4.0, see `LICENSE`.
