# Approaches — process-engineer

Distilled from Superpowers (brainstorming, writing-plans, TDD, subagent-driven-development, systematic-debugging, verification-before-completion), LoopForge DevFlow, and agent-skills (planning, incremental implementation, doubt/constraint/source-driven development, debugging, context-engineering).

## 0. Size the work

| Size | Process |
|------|---------|
| Trivial (typo, rename, one-line) | Do it; skip design gate |
| Small change | Short design (a few lines each: intent, goals/non-goals, approach) → approve → implement with TDD |
| Project / multi-step | Full design doc → plan with tasks → execute → verify |
| Several independent projects | Say so; agree order; brainstorm one at a time |

If scope grows mid-task: stop, say so, step up a size.

## 1. Brainstorm / clarify (no product code)

### Look before you ask
In an existing project, dig in before the first clarifying question. Read what they referred to until you can explain how relevant parts work today and what the change would touch. Never ask what the project already answers.

### First message posture
- If they already specified intent: ~200 words echo (what/who/why), what you found, invite corrections, then one open question if why is missing — or short design if nothing open.
- If underspecified: one open question about the biggest unsettled thing; say what the answer would change.
- If they did not ask for brainstorming: offer a one-line opt-out to just dive in.

### Conversation rules
- Ask only when the answer would change what gets built.
- Ask **one at a time**; plain language; match their vocabulary; no process jargon.
- Until you know **why**, open questions with no example answers. Once you know why, sketch named options with tradeoffs and your pick.
- Ground to cover (territory, not a script): what kind of thing; why now / success; goals, non-goals, anti-goals; prior art; current state; details they care about.
- Play back each understood chunk (~200–300 words); only their words as theirs; your fills as proposals.
- **Lay out approaches in a message of their own** before writing the design: 2–3 real alternatives, tradeoffs, recommend one.
- Spike exception: throwaway build they approved — no tests/plan required; keeping spike output is a new request through the gate.

### Written design
A builder in the domain could plan from it without going back to the human:
- Intent and why
- Goals, non-goals, anti-goals
- Constraints
- Approaches considered + chosen
- How decisions they made
- What's left to the builder

Prefer a durable path such as `docs/specs/YYYY-MM-DD-<topic>-design.md` (user preference overrides).

### HARD GATE
Nothing gets built until design approval: product code, scaffolding, installing deps, creating projects, invoking implementation skills. Reading/exploring OK. Exceptions: user opted out of questions; approved spike (labeled throwaway).

After approval → write the implementation plan (do not skip to coding).

## 2. Writing plans (for a junior agent)

Audience: engineer who has not seen this codebase or spec. Document decisions they cannot know: files, names/signatures, spec values, tests that prove each task.

### Scope check
One plan per independently shippable subsystem. Suggest splitting if the spec covers multiple.

### File structure first
Map create/modify responsibilities before tasks. Prefer focused files; follow existing patterns; split by responsibility not layer.

### Task right-sizing
Smallest unit with its own test cycle worth a fresh reviewer gate. Fold scaffolding into the task that needs it. Each task ends with independently testable deliverable.

### Plan header (required shape)
- Goal (one sentence)
- Architecture (2–3 sentences)
- Tech stack
- Spec path
- Global constraints (verbatim values from spec)
- Review focus (failure modes the spec implies that no task's tests yet cover — then pin tests into owning tasks)

### Task shape
For each task: Files (create/modify/test paths); Interfaces (consumes/produces exact signatures); Steps as checkboxes:
1. Write failing test (assertions as code with spec values)
2. Run to verify fail (command + expected failure)
3. Implement minimal (signature + approach line; body only if algorithm not determined)
4. Run to verify pass
5. Commit (when user wants git)

A step is done when the implementer can write exactly one reasonable thing. A plan longer than the code is a transcript — shrink. Lines that decide nothing (TBD, "handle edge cases") are gaps.

### Self-review before handoff
1. Spec coverage — every requirement → a task
2. Step scan — unambiguous, not over-specified
3. Type/name consistency across tasks
4. Review focus pinned to tests
5. Proportion vs spec length

### Execution handoff
Ask human to confirm plan; choose **subagent-driven** (fresh implementer + reviewer per task) vs **native** (same session implements; one final review). Recommend one with a one-sentence why.

## 3. Incremental / vertical slices (agent-skills)

Prefer vertical slices (one path through stack) over horizontal layers. Contract-first when FE/BE parallel. Risk-first when uncertainty dominates. Each slice: implement → test → verify → commit → next. Leave system working after every slice. Avoid >~100 lines before a verification point.

## 4. TDD iron law (summary — deep detail in `tdd-engineer`)

```
NO PRODUCTION CODE WITHOUT A FAILING TEST FIRST
```

RED (watch fail for the right reason) → GREEN (minimal) → REFACTOR (on green only). Discover the repo's real test commands first. Suite green before "done," not only the new file. Code-before-test → delete and restart (no "keep as reference").

## 5. Subagent-driven development (when available)

- Fresh context per task; never inherit polluted parent history as "review".
- Progress ledger file survives compaction (trust ledger + git log over memory).
- Per task: dispatch implementer → report → task review (spec + quality) → fix loop or complete → next.
- Continuous: do not pause between tasks for "should I continue?"
- Stop only for: irreversible/destructive ops; security-sensitive actions; side effects outside worktree that norms require asking; plan so broken every path is a guess.
- Otherwise: **rulings** recorded in ledger (`Ruling: what — why — cost if wrong`).
- Never parallel implementers on same tree. Final whole-branch review on most capable model when available.
- Subagent output untrusted until reviewed (diff evidence).

## 6. Doubt / constraint / source postures

- **Doubt-driven:** for non-trivial decisions, claim → extract artifact+contract → fresh adversarial review → reconcile → stop (trivial findings / 3 cycles / user override).
- **Constraint-driven:** write project bar (`CONSTRAINTS.md` or equivalent) with numbers; detect stack before interviewing; refuse silent bar-lowering (skipped tests, disables, stubs).
- **Source-driven:** prefer reading existing patterns and docs over inventing; cite sources for non-obvious choices.

## 7. When something goes wrong

Hand off to systematic debugging posture (`debugger`): reproduce → isolate → hypothesize → minimal fix → regression test. Do not spray changes. If ≥3 failed fixes: question architecture with the human.

## 8. Verification before completion

```
NO COMPLETION CLAIMS WITHOUT FRESH VERIFICATION EVIDENCE
```

Identify proving command → run full/fresh → read exit + failures → claim only with evidence. "Should/probably/seems" = stop. Agent "success" reports are not evidence — check diff and re-run.

## 9. DevFlow stage alignment (portable)

For medium/large structured delivery: REQUIREMENT (clarify + user confirm) → DESIGN → PLAN → IMPLEMENT → REVIEW → TEST → optional KNOWLEDGE. Coordinators do not ghost-write isolated stage outputs. Evidence states: passed / failed / blocked / not-run — never blur.

## Anti-patterns
- Menu of what they might want before they describe intent
- Silent defaults never spoken aloud
- Approving an unwritten design ("sounds good" to the idea ≠ design approval)
- Horizontal "all DB then all API then all UI"
- Skipping red observation
- Controller fixing instead of resuming implementer
- Claiming done from vibes
