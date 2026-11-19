# Rules — search-first

1. Check the repo before adding dependencies.
2. Never claim a channel was searched if it was unavailable.
3. Prefer adopt/extend over greenfield utilities.
4. Respect license and security posture of candidates.
5. Do not add a dependency for a few lines when stdlib/project helpers suffice.
## Upstream distillations

### From `everything-claude-code/documentation-lookup`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.

### From `mattpocock-skills/research`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.

### From `ponytail/ponytail`

# Rules (extracted)

- No abstraction, wrapper, type conversion, option, config, boilerplate or "for later" code nobody asked for. Keep values in the form the platform already gives you. Deletion beats addition. Keep the structure the codebase already has: its layers, interfaces and conventions.
