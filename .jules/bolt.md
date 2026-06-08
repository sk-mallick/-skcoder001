## 2026-06-08 - Heroku Widget Cold Starts
**Learning:** Using `herokuapp.com` endpoints for profile widgets like `github-readme-streak-stats` can cause slow initial loads (cold starts), delaying the rendering of the README file.
**Action:** Always prefer Cloudflare/Vercel-backed endpoints like `streak-stats.demolab.com` over Heroku for third-party widget endpoints.
