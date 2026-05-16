## 2024-05-16 - [Lazy Loading Markdown Images]
**Learning:** Even in static, non-rendered Markdown files on GitHub, adding `loading="lazy"` to `<img>` tags below the fold reduces initial bandwidth and improves performance by preventing the browser from eagerly fetching off-screen images until they are needed.
**Action:** Always search for large off-screen `<img>` tags (like stats, activity graphs, or animated GIFs) in long Markdown files, and explicitly apply `loading="lazy"` when optimizing readmes.
