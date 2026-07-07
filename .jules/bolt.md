# Performance Learnings

## 2026-07-07 - Asset Loading Optimization

**Learning:** Using `herokuapp.com` endpoints for stats widgets can cause slow
initial loads due to Heroku's cold start behavior. Additionally, using
`github.com/.../blob/...` with `?raw=true` for images introduces unnecessary
302 redirect latency.
**Action:** Prefer Cloudflare/Vercel-backed endpoints like
`streak-stats.demolab.com` for streak stats, and use direct
`raw.githubusercontent.com` URLs for GitHub repository files to eliminate
redirect latency.
