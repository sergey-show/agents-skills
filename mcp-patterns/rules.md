# Rules — mcp-patterns

1. Never hardcode a single host's tool name into portable skill docs.
2. Validate all tool inputs; fail with structured errors.
3. Do not put secrets in resource URIs or logs.
4. Keep business logic transport-agnostic.
5. Check current protocol docs before copying outdated SDK signatures.
## Upstream distillations

### From `everything-claude-code/mcp-server-patterns`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.
