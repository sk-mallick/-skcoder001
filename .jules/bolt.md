## 2026-05-21 - Replace Heroku-hosted Streak Stats with Demolab CDN
**Learning:** `github-readme-streak-stats.herokuapp.com` is frequently slow due to Heroku cold starts/free tier sleeping. `streak-stats.demolab.com` uses Cloudflare CDN caching, providing significantly faster TTFB for profile visitors.
**Action:** Always prefer `streak-stats.demolab.com` over the Herokuapp domain for streak stats in GitHub profiles.
