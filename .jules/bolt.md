# Performance Learnings

## 2024-07-06 - Avoid Heroku Cold Starts for Streak Stats

**Learning:** Third-party GitHub profile widgets hosted on Heroku
(e.g., `github-readme-streak-stats.herokuapp.com`) can suffer from significant
loading delays due to cold starts, degrading the perceived performance of the
profile page.

**Action:** Prefer using Cloudflare/Vercel-backed alternative endpoints like
`streak-stats.demolab.com` for these widgets to ensure consistently fast load
times and eliminate cold start latency.
