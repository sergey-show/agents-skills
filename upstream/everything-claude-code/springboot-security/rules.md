# Rules (extracted)

- Always hash passwords with BCrypt or Argon2 — never store plaintext
- No secrets in source; load from env or vault
- Never log secrets, tokens, passwords, or full PAN data
