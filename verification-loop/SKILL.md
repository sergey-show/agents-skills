---
id: verification-loop
name: Verification Loop
version: 1.0.0
description: >-
  Evidence-before-claims verification: build, types, lint, tests, security
  greps, diff review — then PASS/FAIL report. Use before PRs, after
  features, or when about to claim done.
role: Verification Lead
category: engineering
triggers:
  - verify
  - verification loop
  - before PR
  - prove it works
  - verification before completion
  - quality gates
capabilities_required:
  - shell.exec
  - test.run
  - git.ops
capabilities_optional:
  - filesystem.read
  - search.code
  - security.scan
  - ask_user
sources:
  - research/everything-claude-code/skills/verification-loop
  - research/superpowers/skills/verification-before-completion
harness: any
---

# Verification Loop

## Role
Evidence before claims, always. Run the project's real gates; read full output; emit PASS/FAIL with evidence. No "should pass."

## When to use
After a feature/refactor; before PR; when quality gates must pass; before any success/completion claim.

## Workflow
1. Discover project commands (don't assume npm).
2. Phase through: build → types → lint → tests (+ coverage if configured) → security greps → diff review.
3. Stop to fix blockers; re-run failed phases fresh.
4. Report PASS/FAIL with commands and excerpts.
5. Target/env acceptance separate from local checks when relevant.

## Done when
All required phases have fresh evidence; failures named; no success language without green output.

## See also
- Related: `process-engineer`, `tdd-engineer`, `ci-cd-engineer`

## Upstream depth

- `skills/upstream/everything-claude-code/verification-loop/`
- `skills/upstream/superpowers/verification-before-completion/`
- `skills/upstream/gstack/verify/`
