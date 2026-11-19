# Browser QA checklist (portable)

## Before interact
- [ ] Correct URL / account / feature flag
- [ ] Snapshot taken; target uid/ref noted
- [ ] Wait condition identified (no blind sleep)

## Coverage
- [ ] Happy path
- [ ] Empty / zero data
- [ ] Validation errors
- [ ] Authz denial
- [ ] Keyboard-only critical path
- [ ] Narrow viewport (≤390) for primary flow

## Evidence package
- [ ] Steps reproducible by a stranger
- [ ] Expected / actual
- [ ] Artifact paths
- [ ] Severity + user impact
