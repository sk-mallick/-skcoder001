# Performance Learnings

## 2024-10-24 - Optimizing Widget and Asset Loading in Markdown

**Learning:** Heroku-hosted endpoints for dynamic GitHub README widgets (like
streak stats) frequently suffer from slow cold starts, delaying render times.
Furthermore, embedding assets using `github.com/owner/repo/blob/...` with
`?raw=true` introduces unnecessary 302 redirect latency compared to raw access.
**Action:** Always prefer edge-cached endpoints like `streak-stats.demolab.com`
over Heroku, and use direct `raw.githubusercontent.com` URLs for repository
assets to minimize TTFB and optimize profile loading speed.
