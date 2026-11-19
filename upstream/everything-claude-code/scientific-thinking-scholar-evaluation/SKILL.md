---
id: everything-claude-code__scientific-thinking-scholar-evaluation
name: scientific-thinking-scholar-evaluation
version: 1.0.0
description: >-
  Structured scholarly-work evaluation for papers, proposals, literature reviews, methods sections, evidence quality, citation support, and research-writing feedback. Use when evaluating academic or scientific work — papers, proposals, methods sections, or evidence quality — against a repeatable rubric.
role: scientific-thinking-scholar-evaluation
category: design
triggers:
  - scientific thinking scholar evaluation
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/scientific-thinking-scholar-evaluation/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: scientific-thinking-scholar-evaluation
---

# scientific-thinking-scholar-evaluation

## Role

Portable distillation of upstream skill `scientific-thinking-scholar-evaluation` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Structured scholarly-work evaluation for papers, proposals, literature reviews, methods sections, evidence quality, citation support, and research-writing feedback. Use when evaluating academic or scientific work — papers, proposals, methods sections, or evidence quality — against a repeatable rubric.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
