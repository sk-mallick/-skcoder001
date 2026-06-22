# Performance Learnings

## 2024-06-22 - Avoid Heroku Cold Starts
**Learning:** Using `github-readme-streak-stats.herokuapp.com` for GitHub Profile README widgets causes slow initial load times due to Heroku's cold start behavior for free-tier apps.
**Action:** Always prefer Cloudflare/Vercel-backed endpoints (e.g., `streak-stats.demolab.com`) to ensure fast and consistent widget loading.

## 2024-06-22 - Avoid 302 Redirects for Images
**Learning:** Embedding images or GIFs in a README using `github.com/.../blob/...` URLs with `?raw=true` introduces unnecessary 302 redirect latency, delaying rendering.
**Action:** Always use the direct `raw.githubusercontent.com/...` URL to serve assets directly and eliminate redirect hops.