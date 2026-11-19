---
id: agent-skills__code-review-and-quality
name: code-review-and-quality
version: 1.0.0
description: >-
  Conducts multi-axis code review. Use before merging any change. Use when reviewing code written by yourself, another agent, or a human. Use when you need to assess code quality across multiple dimensions before it enters the main branch. Use when asked to review a diff or a pull request, even when the diff is pasted inline and the review looks quick to do from reading it.
role: code-review-and-quality
category: security
triggers:
  - code review and quality
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - subagent.spawn
  - test.run
sources:
  - research/agent-skills/skills/code-review-and-quality/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: code-review-and-quality
---

# code-review-and-quality

## Role

Portable distillation of upstream skill `code-review-and-quality` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Conducts multi-axis code review. Use before merging any change. Use when reviewing code written by yourself, another agent, or a human. Use when you need to assess code quality across multiple dimensions before it enters the main branch. Use when asked to review a diff or a pull request, even when the diff is pasted inline and the review looks quick to do from reading it.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
