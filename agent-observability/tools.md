# Tools — agent-observability

## Required
- `filesystem.read` / `filesystem.write` — hook templates, metrics logs, state sidecars

## Optional
- `shell.exec` — smoke hooks
- `ask_user` — privacy/retention choices
- `memory.persist` — aggregate cost digests

## Event contract
| Event | Fields |
|-------|--------|
| session/tool/usage/stop/stage_transition | always `event`, `sid`, `ts` |
| tool | name, duration_ms, ok |
| usage | input/output tokens, cost if known |

## Levels
- **lite** — session start/stop + usage
- **full** (default) — + per-tool latency pairing
- **ultra** — + orchestrator stage attribution
