# Performance Learnings

## 2026-07-01 - Avoid Heroku for widgets
**Learning:** Using `github-readme-streak-stats.herokuapp.com` for widgets
introduces a significant performance bottleneck due to Heroku
cold starts.
**Action:** Prefer Cloudflare/Vercel-backed endpoints like
`streak-stats.demolab.com` for streak stats to ensure fast load times.
