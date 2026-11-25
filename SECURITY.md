# Security Policy

VERIDIUM handles product identity, traceability and regulatory data. We take security reports seriously.

## Reporting a vulnerability

- **Do not open a public issue, discussion or pull request** for a security problem.
- Report it privately to the VERIDIUM maintainers (organization owners of `Veridium-Global`). Where GitHub private vulnerability reporting is enabled for a repository, use **Security → Report a vulnerability**.
- Include: affected repository and version / commit, steps to reproduce, impact, and any proof of concept.

We aim to acknowledge reports within **3 business days** and to agree a fix and disclosure timeline with the reporter.

## Scope

All repositories owned by `Veridium-Global` and the services deployed from them.

## Handling secrets

- Never commit keys, passwords, tokens, certificates or personal data.
- If a secret is committed, treat it as compromised: rotate it first, then remove it from history.
- Use environment variables or the deployment platform's secret store.
