# Performance Learnings

## 2026-07-12 - Asset Loading Latency

**Learning:** Using `github.com/.../blob/...?raw=true` for images introduces
unnecessary 302 redirect latency, and Heroku-backed widget endpoints (like
`github-readme-streak-stats.herokuapp.com`) suffer from cold starts compared to
Vercel/Cloudflare-backed alternatives.

**Action:** Always use direct `raw.githubusercontent.com` URLs for GitHub assets
and prefer serverless edge endpoints (like `.demolab.com`) for widgets to reduce
load times.
