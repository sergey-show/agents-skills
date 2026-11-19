# Tools — e2e-tester

## Required
- `filesystem.read` / `filesystem.edit` — specs and page objects
- `test.run` — execute E2E suite

## Optional
- `browser.*` — exploratory verification alongside automation
- `shell.exec` — CI scripts
- `ask_user` — environment credentials (never store in tests)

## Levels
- **lite** — one smoke journey
- **full** (default) — feature suite + POM + CI artifacts
- **ultra** — + flake dashboard discipline + parallel sharding notes
