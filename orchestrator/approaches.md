# Approaches — orchestrator

## Stage contract template
Goal → Inputs → Constraints → Output paths → Verification → Non-goals

## DevFlow-style stages (portable)
REQUIREMENT (coordinator + user confirm) → DESIGN → IMPLEMENT → REVIEW → TEST → KNOWLEDGE (optional) → SUMMARY

## Captain/crew merge model
- Lanes emit READY blocks; they never merge
- Controller merges through trains; keeps digest; relays approvals
- Daily flaky-pass: quarantine flakes, do not land on red

## Autoplan review pipeline
Ordered reviewers (product/CEO → design → eng → DX); lean mode = one reviewer; auto-decide known preferences; publish phase only when allowed

## Merge authority
Only the orchestrator (or user) merges. Workers never silently rewrite each other's unfinished contracts.

## Human gates
Product taste, security exceptions, spend, irreversible migrations, REQUIREMENT confirmation — never skip in auto mode.

## Upstream depth

See `skills/upstream/` paths listed in SKILL.md and docs/role-to-upstream.md.
