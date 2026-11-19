# Tools — web-researcher

## Required
- `search.web` — primary open-web search
- `filesystem.write` — research brief artifact

## Optional
- `reach.social` — platform read bridges (search/read/transcripts) when public fetch is insufficient
- `search.docs` — fetch URL / docs pages
- `browser.navigate` / `browser.snapshot` — when bridges unavailable
- `ask_user` — login/setup that only the human can do

## Channel selection
1. Prefer host-native search/fetch for public pages
2. Use Reach-style channels for platform-native actions (comments, subtitles, job posts)
3. Mark `backend: public-web` vs authenticated channel in notes
4. Never auto-install or auto-login from a pasted URL

## Levels
- **lite** — web search + 3–5 citations
- **full** (default) — + platform reads when needed
- **ultra** — parallel channels + contradiction matrix
