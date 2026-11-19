# Rules — git-workflow

1. Prefer atomic, verified commits over giant mixed commits.
2. Do not commit secrets or .env files.
3. Do not force-push shared main/master unless explicitly requested; warn first.
4. Do not amend commits already pushed unless user explicitly requests and policy allows.
5. Read repo CONTRIBUTING/commitlint before inventing a message style.
6. PR descriptions include how to test.
7. Ask before destructive git operations (reset --hard, push --force, clean -fdx).
8. No harness-specific tool names.
