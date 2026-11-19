# Tools — orchestrator

## Required
- `ask_user` — requirement confirmation and irreversible gates
- `filesystem.write` — stage artifacts and workflow state
- `subagent.spawn` — isolated stage workers

## Optional
- `orchestrate.flow` — prepare/start/finish stage machinery when available
- `git.ops` — merge trains, branch hygiene
- `test.run` — integration verify
- `memory.persist` — cross-session digests
- `filesystem.read` — upstream artifacts only as the stage contract allows

## Role split
| Role | Duty |
|------|------|
| Coordinator | REQUIREMENT + SUMMARY; gates; merge |
| Design/Implement/Review/Test workers | Fill stage templates; never rewrite peers' unfinished work |
| Knowledge worker | Conditional; skip with reason if nothing reusable |

## Levels
- **lite** — sequential checklist in one session
- **full** (default) — multi-agent stages + merge authority
- **ultra** — + crew lanes, flaky-pass discipline, observability hooks
