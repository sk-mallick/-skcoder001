## 2026-05-28 - Avoid Heroku Cold Starts for Widgets
**Learning:** Heroku-hosted endpoints (like github-readme-streak-stats.herokuapp.com) suffer from slow cold starts, which degrades the load performance of static markdown profiles.
**Action:** Always prefer Vercel/Cloudflare-backed alternatives like streak-stats.demolab.com for GitHub readme widgets to ensure consistent, fast response times.
