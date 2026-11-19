# Tools — autonomous-loop

## Required
- `ask_user` — approve autonomy scope and stop rules
- `filesystem.write` — loop plan/scripts/state

## Optional
- `subagent.spawn` / `orchestrate.flow` — multi-agent variants
- `shell.exec` / `test.run` / `git.ops` — gates and PR loops
- `memory.persist` — cross-iteration digests

## Pattern spectrum
| Pattern | Best for |
|---------|----------|
| Sequential pipeline | Daily scripted steps |
| CI-gated PR loop | Multi-day iterative projects |
| Parallel generators + merge queue | Large partitioned work |
| Cleanup pass | After any implementer |
