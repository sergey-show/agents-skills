# Rules (extracted)

- Do not call or use tools.
- Do not scan or read files.
- Do not run shell commands, provider CLIs, debug logging, or MCP discovery.
2. Never recursively enumerate the workspace root, home directory, provider
3. Never launch a provider CLI, MCP server, or debug session to count tools.
5. Do not write temporary logs or copy configuration content into the report.
