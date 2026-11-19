# Rules — agent-observability

1. Hooks must not block or fail the main agent flow (exit success).
2. Never log secrets, prompts with credentials, or raw PII.
3. Keep timeouts short; drop metrics rather than hang.
4. Always include `event`, `sid`, `ts`.
5. No harness-proprietary metric APIs as hard requirements — describe portable event shapes.
## Upstream distillations

### From `everything-claude-code/agent-introspection-debugging`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.

### From `TokenEconomizer/status`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.
