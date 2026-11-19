# Approaches — ship-gate

## When to escalate vs skip

**Run full gate** when production-bound, user asks go/no-go, or blast radius is non-trivial.

**Tiny-change skip** only if **all** hold: ≤2 files, <50 lines, touches none of auth / payments / data access / config-env. Document the skip rationale in the decision doc.

## Phase A — Fan-out (agent-skills `/ship` portable)

Spawn independent lenses in **one turn** when `subagent.spawn` exists (parallel). Otherwise run sequentially but keep the same merge contract.

| Lens | Ethos / skill | Looks for |
|------|---------------|-----------|
| Code quality | `staff-reviewer` | correctness, readability, architecture, perf axis |
| Security | `security-officer` (guidance) | OWASP, secrets, authz, injection |
| Tests | `qa-lead` / test engineer | happy/edge/error/concurrency gaps |

UI / web changes add:
| A11y | `a11y-auditor` | WCAG AA blockers |
| Webperf | `webperf-auditor` | LCP/CWV regressions on changed paths |

Constraints:
- Specialists do **not** call each other
- Each returns a report only
- Captain owns merge and decision

## Phase B — Merge

1. Promote Critical/High to **blockers**; Important → recommended.
2. Dedupe across lenses; keep highest severity + union of evidence.
3. Captain-direct checks: env vars, migrations, feature flags, monitoring/alerts, README/changelog, rollback affordances.
4. Cross-check code-review security axis vs security report.

## Phase C — Decision

Fill [references/decision-template.md](references/decision-template.md).

- **NO-GO** default if any Critical remains
- User may accept risk only with an explicit sentence recorded under Acknowledged risks
- **Rollback plan is mandatory before GO** (triggers, procedure, RTO)
- On GO + user intent to land → hand off to `release-engineer`

## Definition of done (portable)

- [ ] Changed behavior covered by tests **or** named gap accepted
- [ ] No unresolved Critical security findings
- [ ] Required CI/verify green (list skips with reasons)
- [ ] User-facing docs/changelog updated if behavior changed
- [ ] Migrations/flags/monitoring plan clear
- [ ] A11y/perf considered for UI
- [ ] Rollback path written
- [ ] Owner approval for residual risks

## Evidence hygiene

- Sensitive security detail → summarize safely; keep full detail out of public PR bodies
- Cite artifact paths (test output, audit reports), not vibes
- Never claim GO because "CI is green" alone
