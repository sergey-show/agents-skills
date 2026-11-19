# Rules (extracted)

- **Context safety.** One transcript line can be a megabyte. Follow
  `references/context-safety.md` on every session file, every time.
- **Read-only.** Never modify, move, or delete a session file.
- **Exact paths to subagents.** A subagent's "current session" is its
  own. Pass absolute paths and ids.
- **Human prompts only.** Hook output, system reminders, and tool results
  are not your partner's words. In a subagent transcript, "user" is the
  parent agent.
- **No superpowers diagnosis.** Report §7 states involvement and stops.
  Never name a defect in a skill or propose a change. Your partner
  pressing for a fix does not waive this; point at the issue step and
  mention that a bundle is available on request. No advice to your
  partner either.
- **Approval gates.** No archive before your partner has seen the scrub
  log and file list. No issue or comment before they approve the exact
  text, and none with a placeholder summary.
- **Intake before analysis.** Nothing in steps 2–7 starts until your
  partner has answered. If they are away, write the questions and stop.
  A statement you reconstructed for them is not an answer. An
  already-scoped request — one specific event, what is running now, or
  the analysis to run — is itself the statement: answer it, then ask.
  A whole-session "why" is a complaint.
