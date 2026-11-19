# Approaches — e2e-tester

## Organization
```
tests/e2e/<area>/*.spec.*
tests/fixtures/
pages/ or screen helpers
```

## Stability tactics
- Wait for response/URL/locator state, not `sleep`
- Isolate data per test; no shared mutable accounts when avoidable
- Retry only at CI harness level with cause tracking — do not hide bugs
- Prefer fewer deep E2E + more unit/integration underneath

## Flake triage
Repro locally → classify timing/isolation/env → fix or quarantine with owner → delete obsolete tests

## Upstream depth

See `skills/upstream/` paths listed in SKILL.md and docs/role-to-upstream.md.
