---
id: everything-claude-code__cpp-testing
name: cpp-testing
version: 1.0.0
description: >-
  Use only when writing/updating/fixing C++ tests, configuring GoogleTest/CTest, diagnosing failing or flaky tests, or adding coverage/sanitizers.
role: cpp-testing
category: design
triggers:
  - cpp testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/cpp-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: cpp-testing
---

# cpp-testing

## Role

Portable distillation of upstream skill `cpp-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use only when writing/updating/fixing C++ tests, configuring GoogleTest/CTest, diagnosing failing or flaky tests, or adding coverage/sanitizers.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
