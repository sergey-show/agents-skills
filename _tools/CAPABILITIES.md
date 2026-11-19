# Abstract capabilities (DoT tool vocabulary)

Skills declare these IDs — never harness-specific tool names.

## Filesystem

| ID | Meaning |
|----|---------|
| `filesystem.read` | Read file contents |
| `filesystem.edit` | Create/update/delete files |
| `filesystem.list` | List directories / glob |

## Search

| ID | Meaning |
|----|---------|
| `search.code` | Grep / structural code search |
| `search.web` | Web search |
| `search.docs` | Fetch URL / docs pages |

## Execution

| ID | Meaning |
|----|---------|
| `shell.exec` | Run shell commands in project sandbox |
| `git.ops` | Status, diff, log, commit, branch, PR helpers |
| `test.run` | Run project test / typecheck / lint commands |

## Interaction

| ID | Meaning |
|----|---------|
| `ask_user` | Structured or free-form questions to the human |
| `subagent.spawn` | Launch isolated agent workers |
| `memory.persist` | Save/load cross-session notes |

## Browser & runtime

| ID | Meaning |
|----|---------|
| `browser.navigate` | Open URL / tab |
| `browser.snapshot` | Accessibility tree / DOM snapshot |
| `browser.interact` | Click, type, scroll, select |
| `browser.screenshot` | Visual capture |
| `browser.network` | Inspect network requests |
| `browser.cdp` | Raw DevTools Protocol when needed |

## Domain tools (optional integrations)

| ID | Meaning |
|----|---------|
| `graph.build` | Build knowledge graph from corpus |
| `security.scan` | Static/dynamic security scanners |
| `design.render` | Mockup / design-system renderers |
| `reach.social` | Read X/Reddit/YouTube/GitHub via research bridges |
| `reverse.inspect` | Inspect binaries/apps without source |
| `token.prune` | Prune unused tools / compress context |
| `orchestrate.flow` | Multi-agent stage gates and handoffs |

## Resolution rules for adapters

1. Map each required capability to at least one host tool.
2. If a required capability cannot be mapped, tell the user before proceeding.
3. Optional capabilities: skip silently or note degraded mode.
4. Prefer the host's native tool over spawning external CLIs when equivalent.
