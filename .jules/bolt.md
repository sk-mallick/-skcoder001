## 2026-06-11 - Image Endpoint Optimizations
**Learning:** Using Heroku endpoints (like `github-readme-streak-stats.herokuapp.com`) causes slow cold starts for widgets. Embedding GitHub repository files via `github.com/user/repo/blob/master/file?raw=true` introduces unnecessary 302 redirect latency.
**Action:** Prefer Cloudflare/Vercel-backed endpoints (e.g., `streak-stats.demolab.com`) for widgets. Always use direct `raw.githubusercontent.com` URLs for embedding GitHub files to improve load times.
