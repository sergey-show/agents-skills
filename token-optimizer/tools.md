# Tools — token-optimizer

## Required
- `filesystem.read` — inspect configs, skill lists, session notes
- `ask_user` — approve prune/apply/restore

## Optional
- `token.prune` — show/measure/apply/restore unused-tool deny lists
- `memory.persist` — store micro-skills / fact pins across sessions
- `shell.exec` / `filesystem.write` — emit lean profiles and reports

## Operations
| Op | Meaning |
|----|---------|
| show | Current prune proposal / deny list |
| measure | Estimated savings vs capability risk |
| apply | Write deny list (user-approved) |
| restore | Undo prune (user-approved) |
| microskills | List learned short facts injected at session start |

## Levels
- **lite** — advisory inventory only
- **full** (default) — + prune proposal + micro-skill extraction
- **ultra** — + loop-guard envelope tuning
