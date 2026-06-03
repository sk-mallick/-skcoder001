## 2026-06-03 - Avoid Heroku Cold Starts for GitHub Widgets
**Learning:** Widgets hosted on Heroku (like github-readme-streak-stats.herokuapp.com) suffer from slow cold starts, significantly delaying image rendering on profile pages.
**Action:** Prefer Cloudflare/Vercel-backed endpoints (e.g., streak-stats.demolab.com) instead for faster, more reliable loading times.
