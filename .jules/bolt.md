# Performance Learnings

## 2026-06-19 - Avoid Heroku Cold Starts for Streak Stats

**Learning:** Third-party GitHub profile widgets hosted on Heroku (like
github-readme-streak-stats.herokuapp.com) often suffer from slow cold starts,
increasing image load times.

**Action:** Prefer Cloudflare/Vercel-backed endpoints (e.g.,
streak-stats.demolab.com) to avoid slow cold starts and improve load times.
