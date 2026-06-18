## 2024-06-18 - Heroku Cold Starts on Profile Badges
**Learning:** Using herokuapp.com endpoints for GitHub profile badges
introduces significant latency due to Heroku's cold start behavior.
**Action:** Always prefer Vercel or Cloudflare-backed endpoints like
streak-stats.demolab.com over Heroku for third-party stats widgets.
