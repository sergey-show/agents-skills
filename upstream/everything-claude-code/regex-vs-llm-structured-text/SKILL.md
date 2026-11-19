---
id: everything-claude-code__regex-vs-llm-structured-text
name: regex-vs-llm-structured-text
version: 1.0.0
description: >-
  Decision framework for parsing structured text (quizzes, forms, invoices, receipts, tables) with a hybrid regex-first pipeline — regex extraction handles 95%+ cheaply, a confidence scorer flags low-confidence items, and an LLM validator fixes only the edge cases. Use when choosing between regex and LLM for text extraction, building a cheap document parser, or optimizing extraction cost and accuracy.
role: regex-vs-llm-structured-text
category: engineering
triggers:
  - regex vs llm structured text
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/regex-vs-llm-structured-text/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: regex-vs-llm-structured-text
---

# regex-vs-llm-structured-text

## Role

Portable distillation of upstream skill `regex-vs-llm-structured-text` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Decision framework for parsing structured text (quizzes, forms, invoices, receipts, tables) with a hybrid regex-first pipeline — regex extraction handles 95%+ cheaply, a confidence scorer flags low-confidence items, and an LLM validator fixes only the edge cases. Use when choosing between regex and LLM for text extraction, building a cheap document parser, or optimizing extraction cost and accuracy.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
