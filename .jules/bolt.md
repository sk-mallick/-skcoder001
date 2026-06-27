# Performance Learnings

## 2024-06-27 - Third-Party Widget and Redirect Latency

**Learning:** Third-party widgets hosted on Heroku
(e.g., `github-readme-streak-stats.herokuapp.com`) can suffer from significant
cold start delays. Additionally, embedding GitHub files using
`github.com/.../blob/...` incurs an unnecessary 302 redirect.

**Action:** Prefer edge-backed endpoints (e.g., `streak-stats.demolab.com`)
and direct `raw.githubusercontent.com` URLs to eliminate latency.
