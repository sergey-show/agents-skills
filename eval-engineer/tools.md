# Tools — eval-engineer

## Required
- `filesystem.write` — eval specs, results, spend tables
- `ask_user` — approve paid pilots and human grades

## Optional
- `filesystem.read` — baselines and prior results
- `shell.exec` / `test.run` — code-based graders
- `subagent.spawn` — parallel arms

## Levels
- **lite** — checklist capability eval
- **full** (default) — capability + regression + pass@k
- **ultra** — preregistered multi-arm paid plan with stop rules
