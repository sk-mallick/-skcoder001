## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-06-04 - Empty Links on Markdown Badges
**Learning:** Wrapping markdown badges or images in empty links (`[![alt](src)]()`) creates confusing, un-navigable tab stops for keyboard users and screen readers, violating accessibility best practices and MD042.
**Action:** Always use plain image tags (`![alt](src)`) for badges or images that do not have a valid destination URL, ensuring better keyboard navigation experience.
