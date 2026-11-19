---
id: agent-skills__ci-cd-and-automation
name: ci-cd-and-automation
version: 1.0.0
description: >-
  Automates CI/CD pipeline setup. Use when setting up or modifying build and deployment pipelines. Use when you need to automate quality gates, configure test runners in CI, or establish deployment strategies.
role: ci-cd-and-automation
category: research
triggers:
  - ci cd and automation
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/agent-skills/skills/ci-cd-and-automation/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: ci-cd-and-automation
---

# ci-cd-and-automation

## Role

Portable distillation of upstream skill `ci-cd-and-automation` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Automates CI/CD pipeline setup. Use when setting up or modifying build and deployment pipelines. Use when you need to automate quality gates, configure test runners in CI, or establish deployment strategies.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
