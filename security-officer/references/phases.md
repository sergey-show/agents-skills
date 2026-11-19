# Security audit phases (portable)

## Schemas / artifacts (conceptual)

| Artifact | Owner | Purpose |
|----------|-------|---------|
| run-metadata | parent | target, ref, profile, budget, status |
| architecture.md | parent | ≤~1000 words model summary |
| coverage-ledger | parent | units: surface × boundary × subsystem × attack class |
| findings | parent | confirmed / needs_validation only after verify |
| REPORT | parent | human summary + gaps |

Unit states (typical): `planned` → `in_progress` → `candidate` / `covered` / `deferred` / `blocked` / `out_of_scope`.

## Profiles

- **quick** — coarsened units; one hunter wave; one critic; partial by design
- **standard** — default workflow
- **deep** — finer units; critic until clean; separate final verification

Scoped runs seed in-scope units and mark the rest `out_of_scope` (never "covered").

## RECON outputs

Product type, stack, entry surfaces, principals, controls, source-to-sink paths, offline test affordances, missing sandbox capabilities.

## HUNT method (summary)

Name principal → accepted input/action → intended control → post-decision path → smallest boundary result → source-level fix + regression. Sad paths and control disagreements matter. See `security-hunter` for deep hunting detail.

## VALIDATE

Independent agent/pass. Bounded local evidence only inside sandbox. No live probing of shared infra.

## REPORT

Severity, evidence, impact, fix, coverage statement. Partial budget exhaustion → incomplete status with fingerprints still candidates.
