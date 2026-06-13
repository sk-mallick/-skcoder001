## 2026-06-13 - External Asset Loading Latency
**Learning:** Widgets hosted on Heroku
(like github-readme-streak-stats.herokuapp.com) experience slow cold starts
that delay rendering. Additionally, using GitHub blob URLs with ?raw=true
introduces an unnecessary 302 redirect.
**Action:** Use Vercel/Cloudflare-backed endpoints like
streak-stats.demolab.com and direct raw.githubusercontent.com URLs to
eliminate latency and redirects.
