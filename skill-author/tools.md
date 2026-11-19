# Tools — skill-author

## Required
- `filesystem.read` / `filesystem.write` — skill files + format/manifest
- `ask_user` — purpose/trigger confirmation

## Optional
- `search.code` — find duplicate skills
- `subagent.spawn` — pressure-test scenarios
- `shell.exec` — lint/count lines

## DoT file set
| File | Load | Holds |
|------|------|-------|
| SKILL.md | always on use | role, when, workflow summary |
| tools.md | on demand | capabilities + levels |
| approaches.md | on demand | methodology |
| rules.md | on demand | never-violate constraints |
