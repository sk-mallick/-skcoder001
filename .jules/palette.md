## 2024-05-24 - Missing Alt Text on Dynamic GitHub Profile Badges
**Learning:** Automatically generated GitHub profile badges, statistics charts, and banners often lack `alt` text when copy-pasted directly from generation tools, causing major screen-reader accessibility issues on otherwise well-structured profile readmes.
**Action:** Always verify `img` tags have descriptive `alt` text, even for dynamic or auto-generated content. If an image is purely decorative, use `alt=""` or `role="presentation"`.
