## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2026-06-06 - Empty Link Badges & Streak Stats
**Learning:** Wrapping images/badges in empty links `[]()` creates accessibility issues for screen readers and triggers markdown linting errors (MD042). Additionally, using `github-readme-streak-stats.herokuapp.com` causes poor UX due to slow Heroku cold starts.
**Action:** Use plain image tags instead of empty links for static badges, and prefer Cloudflare/Vercel-backed endpoints (e.g., `streak-stats.demolab.com`) for faster loading times.
