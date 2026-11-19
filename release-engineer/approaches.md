# Approaches — release-engineer

## Ship workflow (gstack portable)

1. **Preflight:** branch name, base, dirty tree, CI status, VERSION/CHANGELOG needs.
2. **Sync base** without destroying local work; never force-push protected defaults.
3. **Measure:** run targeted then broader tests; record what ran and what was skipped (with reason).
4. **Review the diff** for user-facing behavior, migrations, flags, secrets.
5. **Docs:** changelog / release notes when user-visible behavior changed.
6. **PR:** short summary (why), test plan, risk notes; no secret paste.
7. **Land:** merge only on explicit request; wait CI; deploy if that is the repo's path.
8. **Health:** smoke critical paths; report outcome + rollback hint.

## Land and deploy

Merge → wait CI/deploy → production/staging health smoke → report. Prefer feature flags for risky rolls. If health fails: stop, do not "push through," propose rollback.

## Agent-skills shipping portable

For production-bound changes with non-trivial blast radius, escalate to `ship-gate` fan-out:
- code quality / correctness
- security
- test coverage
Then merge decision + mandatory rollback plan.

Skip full fan-out only when change is tiny (≤2 files, <50 lines) and touches none of: auth, payments, data access, config/env.

## Git parts (portable discipline)

- Status + diff + log before commit messaging
- Conventional, why-focused commit messages when asked to commit
- No `--no-verify` / force / amend of others' commits unless user explicitly orders
- Redact credentials from commit and PR bodies
- Prefer small reviewable PRs; split when the diff mixes unrelated concerns

## Document release

When only docs ship: still verify links/build if the project has a docs pipeline; note doc-only in the PR.
