## 2024-06-09 - Asset Loading Optimizations
**Learning:** Third-party widgets hosted on Heroku (like `github-readme-streak-stats`) suffer from significant cold start delays. Additionally, using `github.com` URLs with `?raw=true` for images incurs unnecessary 302 redirect latency compared to direct `raw.githubusercontent.com` URLs.
**Action:** Use Cloudflare/Vercel-backed endpoints (e.g., `streak-stats.demolab.com`) for streak widgets and always use `raw.githubusercontent.com` for direct GitHub asset embedding to minimize load times.
