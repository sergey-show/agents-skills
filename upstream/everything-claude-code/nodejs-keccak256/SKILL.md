---
id: everything-claude-code__nodejs-keccak256
name: nodejs-keccak256
version: 1.0.0
description: >-
  Prevent Ethereum hashing bugs in JavaScript and TypeScript. Node's sha3-256 is NIST SHA3, not Ethereum Keccak-256, and silently breaks selectors, signatures, storage slots, and address derivation. Use when hashing for Ethereum in JavaScript or TypeScript, or when a selector, signature, storage slot, or derived address is wrong.
role: nodejs-keccak256
category: engineering
triggers:
  - nodejs keccak256
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/nodejs-keccak256/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: nodejs-keccak256
---

# nodejs-keccak256

## Role

Portable distillation of upstream skill `nodejs-keccak256` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Prevent Ethereum hashing bugs in JavaScript and TypeScript. Node's sha3-256 is NIST SHA3, not Ethereum Keccak-256, and silently breaks selectors, signatures, storage slots, and address derivation. Use when hashing for Ethereum in JavaScript or TypeScript, or when a selector, signature, storage slot, or derived address is wrong.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
