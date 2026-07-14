# Performance Learnings

## 2026-07-14 - Avoiding Heroku Cold Starts and Blob Redirects

**Learning:** Using `github-readme-streak-stats.herokuapp.com` for widgets
suffers from severe Heroku cold start latency, and embedding GitHub files via
`blob` URLs with `?raw=true` introduces unnecessary 302 redirects.
**Action:** Always prefer Cloudflare/Vercel-backed endpoints like
`streak-stats.demolab.com` and use direct `raw.githubusercontent.com` URLs
for embedding files to ensure immediate loading.
