# Contributing to VERIDIUM

These rules apply to every repository in `Veridium-Global` unless the repository has its own `CONTRIBUTING.md` or `CLAUDE.md`, which take precedence.

## Workflow

1. **Never push directly to `main`.** Every change goes through a branch and a pull request.
2. Branch from `main`: `<module>/<step-or-ticket>-<short-name>`, for example `freight/4.6-global-map`.
3. Keep pull requests small and focused: one step or ticket per PR.
4. Link the Jira issue (project `KAN`) in the PR title or description: `... (KAN-123)`.
5. Run the repository's checks before opening the PR; describe how you validated the change.
6. At least one review from a code owner or organization owner before merge (unless a standing permission in the repository's instructions says otherwise).
7. Use **Squash and merge**, then delete the branch.

## Commits

- Format: `<module>: <what changed> (KAN-<id>)`.
- Write in the imperative, keep the subject under ~72 characters.

## Architecture rules

- **Contracts, not code:** modules talk to each other only through versioned contracts (`Link`, `Global/contracts`).
- **One concept, one owner:** check the glossary before introducing a new term.
- **Country-specific logic lives in Country Packs**, product-specific logic in Product Category Packs, never in the core.
- Mark mock data as **mock** and simulated flows as **DEMO**; legal, tariff and customs facts need an official source.

## Security

See [SECURITY.md](SECURITY.md). Never commit secrets or personal data.
