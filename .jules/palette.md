## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2025-02-14 - Avoid Empty Links for Badges
**Learning:** Wrapping badges or images in empty markdown links (`[![alt](src)]()`) traps screen reader focus, creating confusing empty navigation points for visually impaired users while triggering markdownlint errors (MD042).
**Action:** Use plain image tags (`![alt](src)`) for purely decorative or informational badges that do not need to link anywhere.
