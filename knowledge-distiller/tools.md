# Tools — knowledge-distiller

## Required
- `filesystem.read` — upstream stage artifacts
- `filesystem.write` — append knowledge notes

## Optional
- `memory.persist` — cross-harness memory vault when available
- `ask_user` — confirm canonical knowledge path
- `search.code` — ground patterns in real modules

## Levels
- **lite** — 3–5 bullets from the latest diff/review
- **full** (default) — categorized append from full stage set
- **ultra** — + dedupe against historical knowledge + memory sync
