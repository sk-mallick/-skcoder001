## 2026-06-10 - Markdown Image Load Performance Optimization
**Learning:** In GitHub markdown profiles, using `github-readme-streak-stats.herokuapp.com` leads to slow load times due to Heroku cold starts. Similarly, embedding images via `github.com/.../blob/...?raw=true` causes unnecessary 302 redirect latency.
**Action:** Replaced the Heroku endpoint with `streak-stats.demolab.com` (a Cloudflare/Vercel-backed endpoint) and changed GitHub blob image URLs to use the direct `raw.githubusercontent.com` URL to eliminate redirects and improve load performance.
