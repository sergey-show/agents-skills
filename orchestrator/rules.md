# Rules — orchestrator

1. Never skip user confirmation on REQUIREMENT for medium/large work.
2. Never let workers merge to shared trunks or overwrite peer artifacts.
3. Protect user changes: no unauthorized stash/commit/push/deploy.
4. Announce completion only from real commands/observations; distinguish passed/failed/blocked/not-run.
5. Do not inject all specialty rules — only evidence-matched profiles.
6. Knowledge stage is conditional; skip with written reason, do not fake entries.
7. Single-context degrade only when host cannot spawn workers — record the reason.
8. No harness-specific executor IDs as portable requirements.
## Upstream distillations

### From `LoopForge/devflow`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.

### From `gstack/autoplan`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.

### From `gstack/captain`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.

### From `superpowers/subagent-driven-development`

# Rules (extracted)

- Never dispatch multiple implementation subagents in parallel (conflicts).
- Do not add open-ended directives like "check all uses" or "run race tests
- Do not ask a reviewer to re-run tests the implementer already ran on the
- Do not pre-judge findings for the reviewer — never instruct a reviewer to

### From `superpowers/dispatching-parallel-agents`

# Rules (extracted)

- No shared state between investigations

### From `agent-skills/using-agent-skills`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.
