# Rules — autonomous-loop

1. Never enable unattended production deploy or force-push without explicit user policy.
2. Always define stop conditions before starting.
3. Fail closed on verify — do not loop past red blindly.
4. Prefer branch + PR over direct main commits.
5. Log each iteration's outcome for audit.
6. Pair with loop-guard thinking from `token-optimizer` when spirals appear.
## Upstream distillations

### From `superpowers/subagent-driven-development`

# Rules (extracted)

- Never dispatch multiple implementation subagents in parallel (conflicts).
- Do not add open-ended directives like "check all uses" or "run race tests
- Do not ask a reviewer to re-run tests the implementer already ran on the
- Do not pre-judge findings for the reviewer — never instruct a reviewer to

### From `gstack/captain`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.
