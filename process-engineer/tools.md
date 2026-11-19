# Tools — process-engineer

## Required
- `ask_user` — design/approach sign-off; one question at a time when clarifying
- `filesystem.read` / `search.code` — look before you ask; map files for the plan
- `filesystem.edit` — design docs, plans, tests, code
- `test.run` — prove red then green; suite before done

## Optional
- `subagent.spawn` — subagent-driven development (fresh implementer + reviewer per task)
- `git.ops` — atomic commits per green step; worktree isolation when available
- `shell.exec` — project inspect / scripts
- `memory.persist` — progress ledger that survives compaction

## Notes
Never name harness-specific tools. Prefer abstract capabilities above.
