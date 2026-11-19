---
id: everything-claude-code__bengali-nlp
name: bengali-nlp
version: 1.0.0
description: >-
  Bengali (Bangla) text processing patterns including Unicode normalization, script detection, tokenization, conjunct handling, and Bangla-specific NLP best practices for AI applications.
role: bengali-nlp
category: engineering
triggers:
  - bengali nlp
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/bengali-nlp/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: bengali-nlp
---

# bengali-nlp

## Role

Portable distillation of upstream skill `bengali-nlp` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Bengali (Bangla) text processing patterns including Unicode normalization, script detection, tokenization, conjunct handling, and Bangla-specific NLP best practices for AI applications.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
