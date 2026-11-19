---
id: everything-claude-code__article-writing
name: article-writing
version: 1.0.0
description: >-
  Write articles, guides, blog posts, tutorials, newsletter issues, and other long-form content in a distinctive voice derived from supplied examples or brand guidance. Use when the user wants polished written content longer than a paragraph, especially when voice consistency, structure, and credibility matter.
role: article-writing
category: research
triggers:
  - article writing
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - shell.exec
sources:
  - research/everything-claude-code/.agents/skills/article-writing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: article-writing
---

# article-writing

## Role

Portable distillation of upstream skill `article-writing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Write articles, guides, blog posts, tutorials, newsletter issues, and other long-form content in a distinctive voice derived from supplied examples or brand guidance. Use when the user wants polished written content longer than a paragraph, especially when voice consistency, structure, and credibility matter.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
