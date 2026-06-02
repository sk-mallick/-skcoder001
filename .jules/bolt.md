## 2026-06-02 - Optimize Asset Load Latency
**Learning:** Using `github-readme-streak-stats.herokuapp.com` incurs significant Heroku cold-start latency, and using `github.com/.../blob/...` with `?raw=true` introduces unnecessary 302 redirects for assets.
**Action:** Prefer Cloudflare/Vercel-backed endpoints like `streak-stats.demolab.com` for streak stats and direct `raw.githubusercontent.com` URLs for raw GitHub assets to significantly improve profile load times.
