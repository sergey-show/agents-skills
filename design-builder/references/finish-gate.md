# Finish gate states (portable)

| State | Meaning | Agent action |
|-------|---------|--------------|
| PASS | No blocking FAILs | Finish; record evidence |
| FAIL n (round k/max) | Fixable blockers | Fix listed items; re-run |
| OPEN n | Rounds used up | List FAILs + waivers; stop grinding |
| QUICK | Mid-look, not a round | Informative only |
| SETUP | No openable target | Arm URL/file; retry |
| ERROR / OFF | Tooling/no build | Report; don't loop |
| DONE (user words) | User ended | Record words + open FAILs |

Waivers JSON shape (conceptual): `{ "check", "target", "reason" }` with reason ≥12 chars. kit-integrity / checker-gaming style issues are non-waivable.
