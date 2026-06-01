## 2026-06-01 - Avoid Heroku endpoints for GitHub README widgets
**Learning:** Heroku-hosted widgets like `github-readme-streak-stats.herokuapp.com` suffer from slow cold starts, negatively impacting the load time of static GitHub profiles.
**Action:** Prefer Cloudflare or Vercel-backed instances like `streak-stats.demolab.com` for faster, more reliable rendering.
