---
id: everything-claude-code__visa-doc-translate
name: visa-doc-translate
version: 1.0.0
description: >-
  Translate visa document images (bank deposit, employment, income, and retirement certificates; HEIC, PNG, or JPG) into English via OCR and produce a bilingual PDF pairing the original image with a formatted certified-style translation. Use when a visa application needs a document translated to English, an official certificate OCR'd and translated, or a bilingual translation PDF for immigration paperwork.
role: visa-doc-translate
category: engineering
triggers:
  - visa doc translate
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/visa-doc-translate/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: visa-doc-translate
---

# visa-doc-translate

## Role

Portable distillation of upstream skill `visa-doc-translate` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Translate visa document images (bank deposit, employment, income, and retirement certificates; HEIC, PNG, or JPG) into English via OCR and produce a bilingual PDF pairing the original image with a formatted certified-style translation. Use when a visa application needs a document translated to English, an official certificate OCR'd and translated, or a bilingual translation PDF for immigration paperwork.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
