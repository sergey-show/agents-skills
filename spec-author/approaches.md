# Approaches — spec-author

Distilled from Spec-Kit templates/commands, agent-skills spec-driven-development, Matt Pocock (grill→to-spec→to-tickets→implement*), interview-me, idea-refine. Host wiring stripped.

## Pipeline (Spec-Kit aligned)
Idea → **specification** → **implementation plan** → **task list**. Do not skip code-reading in the technical phase. Constitution (project principles) constrains all specs when present.

## Five phases
1. **Why** — problem, users, success metric; refuse solutioning before problem is crisp.
2. **Scope** — in / out / later; non-goals and anti-goals.
3. **Technical** — mandatory code reading; interfaces; data; risks; prefer existing seams.
4. **Draft** — reviewable in one sitting; chunk for sign-off if long.
5. **File** — persist + link tasks; status Draft until approved.

## Interview → Spec (Matt Pocock / interview-me)
- If intent is fuzzy: run `interviewer` posture first (or idea-refine for variations).
- **to-spec posture:** when conversation already has enough context — **do not re-interview**; synthesize. Explore repo; use domain glossary; respect ADRs.
- Sketch **test seams** first; prefer existing seams; highest seam possible; fewer seams better (ideal: one). Confirm seams with user before locking the spec.
- Spec template sections:
  - Problem Statement (user perspective)
  - Solution (user perspective)
  - User Stories (extensive numbered list: As an… I want… so that…)
  - Implementation Decisions (modules, interfaces, schema, API contracts — **no fragile file paths/snippets** unless prototype encodes a decision)
  - Testing Decisions (external behavior only; modules; prior art)
  - Out of Scope
  - Further Notes

## Spec-Kit feature specification shape
- Header: feature name, branch `###-feature-name`, date, status, input description
- **User Scenarios & Testing (mandatory):** prioritized user journeys (P1, P2, …), each independently testable MVP slice
  - Why this priority
  - Independent Test
  - Acceptance Scenarios: Given / When / Then
- Edge Cases
- Requirements / success criteria measurable
- Assumptions and open questions

## Plan template alignment
After spec approval, implementation plan covers: technical context, constitution check, architecture, phases, complexity tracking — or hand to `process-engineer` / `eng-architect` for deep planning.

## Tasks template alignment
- Checkbox tasks ordered by dependency
- Each task maps to acceptance scenarios
- Parallelizable tasks marked
- Include test tasks, not only code tasks

## Idea-refine (when brainstorming product shape)
Generate constrained variations; force tradeoffs; pick a wedge before writing the full spec. Do not expand into a platform vision without an explicit wedge story.

## to-tickets
Break signed spec into tickets/tasks: one vertical slice or one acceptance cluster per ticket; include test notes; avoid tickets that only say "implement the spec."

## implement* handoff
Specs do not include brittle file paths. Implementers read spec + plan; process-engineer owns TDD execution. Spec author may clarify language but does not silently change approved scope.

## Chunked sign-off
Present digestible sections; get explicit approval. "Looks good" on an unread section is not approval — confirm what they reviewed.
