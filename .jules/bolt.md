## 2026-05-30 - Optimize third-party widget and asset loading
**Learning:** Using Heroku-backed endpoints (like `github-readme-streak-stats.herokuapp.com`) for GitHub profile widgets introduces significant loading delays due to Heroku cold starts. Additionally, using `github.com/.../blob/...?raw=true` URLs for assets introduces unnecessary 302 redirect latency.
**Action:** Always prefer Cloudflare/Vercel-backed endpoints (e.g., `streak-stats.demolab.com`) for widgets, and use direct `raw.githubusercontent.com` URLs for GitHub-hosted assets to ensure immediate loading.
