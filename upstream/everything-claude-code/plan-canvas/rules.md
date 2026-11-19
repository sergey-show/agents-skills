# Rules (extracted)

- Markdown artifacts render in ECC's plan template (including Mermaid blocks);
  `.html` artifacts render as-is with the annotation layer injected. For HTML
  authoring guidance use the `frontend-design-direction` and `artifact-design`
  skills.
- Edit the artifact file to revise — the canvas live-reloads on save. Never
  re-run `open` to refresh.
- `{"status": "ended", "endedBy": "user"}` (or `sessionEnded: true` on a
  feedback batch) means the user closed the review: stop polling, deliver
  remaining updates in chat, and do not reopen. A plain `open` on that
  session is refused; pass `--reopen` only when the user asks to resume.
- Sibling assets (images, CSS) must sit next to the artifact and be
  referenced by relative path.
- The server is loopback-only and exits after 30 idle minutes
  (`ECC_PLAN_CANVAS_IDLE_MS`); `stop` shuts it down explicitly. State lives
  in ``<agent-skills-dir>/...`` (`ECC_PLAN_CANVAS_STATE_DIR`).
