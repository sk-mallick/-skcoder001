
## 2026-06-07 - Image Load Latency in Markdown
**Learning:** GitHub profile READMEs suffer from slow TTFB when relying on Heroku-backed widgets (`github-readme-streak-stats.herokuapp.com`) due to cold starts, and experience unnecessary 302 redirect latency when using `github.com/username/repo/blob/branch/file?raw=true` instead of direct raw URLs.
**Action:** Always prefer Cloudflare/Vercel-backed endpoints like `streak-stats.demolab.com` for widgets, and use `raw.githubusercontent.com` directly for GitHub-hosted assets.
