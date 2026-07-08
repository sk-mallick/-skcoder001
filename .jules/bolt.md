# Performance Learnings

## 2026-07-08 - Avoid Heroku Cold Starts

**Learning:** Using Heroku-backed endpoints for streak stats causes slow profile
load times due to cold starts.
**Action:** Prefer Cloudflare/Vercel-backed endpoints like demolab.com for widgets.
