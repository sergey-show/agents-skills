---
id: everything-claude-code__scientific-thinking-literature-review
name: scientific-thinking-literature-review
version: 1.0.0
description: >-
  Systematic literature-review workflow for academic, biomedical, technical, and scientific topics, including search planning, source screening, synthesis, citation checks, and evidence logging. Use when the task is to find, screen, synthesize, and cite a body of academic or technical literature.
role: scientific-thinking-literature-review
category: research
triggers:
  - scientific thinking literature review
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
sources:
  - research/everything-claude-code/skills/scientific-thinking-literature-review/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: scientific-thinking-literature-review
---

# scientific-thinking-literature-review

## Role

Portable distillation of upstream skill `scientific-thinking-literature-review` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Systematic literature-review workflow for academic, biomedical, technical, and scientific topics, including search planning, source screening, synthesis, citation checks, and evidence logging. Use when the task is to find, screen, synthesize, and cite a body of academic or technical literature.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
