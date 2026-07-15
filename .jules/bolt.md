# Performance Learnings

## 2024-07-15 - Heroku Cold Starts

**Learning:** GitHub profile widgets hosted on Heroku often suffer from slow
cold starts, which delays image loading.

**Action:** Use Vercel or Cloudflare-backed alternatives (like
streak-stats.demolab.com instead of
github-readme-streak-stats.herokuapp.com) to improve profile
load performance.
