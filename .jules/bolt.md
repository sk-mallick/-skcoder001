## 2026-06-05 - Third-Party Widget Latency in Markdown Profiles
**Learning:** Using Heroku-backed endpoints (`herokuapp.com`) for GitHub profile widgets (like streak stats) introduces significant latency due to cold starts compared to Cloudflare/Vercel-backed endpoints. Additionally, embedding GitHub assets via `/blob/...?raw=true` causes unnecessary 302 redirect latency.
**Action:** Always prefer Edge-cached, serverless endpoints like `streak-stats.demolab.com` over Heroku for widgets, and use direct `raw.githubusercontent.com` paths for GitHub-hosted assets to eliminate redirect overhead.
