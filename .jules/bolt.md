## 2026-06-04 - Markdown Image Loading Performance
**Learning:** Using third-party image endpoints on Heroku (e.g., github-readme-streak-stats.herokuapp.com) leads to slow cold starts, and embedding GitHub files via blob URLs with `?raw=true` adds unnecessary 302 redirect latency.
**Action:** Use Vercel/Cloudflare-backed endpoints (like streak-stats.demolab.com) for widgets, and always use direct raw.githubusercontent.com URLs for embedded GitHub files to improve README render speed.
