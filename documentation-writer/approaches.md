# Approaches — documentation-writer

Distilled from agent-skills documentation-and-adrs, gstack document-generate / document-release (portable content; strip host telemetry).

## Choose the artifact
| Need | Artifact |
|------|----------|
| Why we chose X over Y | ADR |
| How to do a task | How-to / runbook |
| What exists / API | Reference |
| What changed in a version | Release notes / changelog |

## ADR template
- Title, status (Proposed/Accepted/Deprecated/Superseded), date, deciders
- Context
- Decision
- Alternatives considered
- Consequences (positive/negative)
- Related ADRs

Never delete an accepted ADR — supersede with a new one.

## Doc quality bar
- Commands copy-pastable and verified
- Paths exist
- Distinguish required vs optional
- Call out pitfalls
- Prefer short pages with links over monoliths

## Release documentation
- Derive from actual commits/PRs/tags when possible
- Separate breaking changes, features, fixes
- Do not claim unverified behavior
- Migration links for breaks (`migration-engineer`)

## document-generate posture
When asked to generate missing docs: inventory code surfaces; draft only what evidence supports; mark unknowns explicitly rather than inventing.
