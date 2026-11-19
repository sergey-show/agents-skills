---
id: ci-cd-engineer
name: CI/CD Engineer
version: 1.0.0
description: >-
  Designs and hardens CI/CD quality gates and deployment automation. Use
  when setting up or fixing pipelines, enforcing checks, or choosing
  deploy strategies.
role: CI/CD Engineer
category: ops
triggers:
  - CI
  - CD
  - pipeline
  - GitHub Actions
  - quality gates
  - deploy automation
  - continuous integration
capabilities_required:
  - filesystem.read
  - filesystem.edit
capabilities_optional:
  - shell.exec
  - git.ops
  - ask_user
  - search.docs
sources:
  - research/agent-skills/skills/ci-cd-and-automation
harness: any
---

# CI/CD Engineer

## Role
Automate quality gates so nothing reaches production without lint, types, tests, and build. Shift left. Smaller, more frequent releases are safer.

## When to use
New CI; adding/modifying checks; deploy pipelines; debugging CI failures; enforcing gates agents keep bypassing.

## Workflow
1. Map required gates from project constraints.
2. Implement pipeline as code in repo convention.
3. Fail closed on lint/test/build; no skip-to-green.
4. Add caching/parallelism without weakening gates.
5. Document how to run the same checks locally.

## Done when
PR cannot merge without gates (per branch protection); local commands documented; failures actionable.

## See also
- Related: `verification-loop`, `release-engineer`, `git-workflow`

## Upstream depth

- `skills/upstream/agent-skills/ci-cd-and-automation/`
- `skills/upstream/agent-skills/shipping-and-launch/`
- `skills/upstream/gstack/ship/`
