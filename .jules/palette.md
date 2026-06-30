## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-06-30 - Avoid empty links for images/badges
**Learning:** Wrapping images or badges in empty links (e.g., `[![alt](src)]()`) creates accessibility issues for screen readers, which announce them confusingly and reload the page on click, and also causes markdown linting errors (MD042).
**Action:** Use plain image tags (`![alt](src)`) instead of wrapping them in empty links when displaying visual elements in GitHub markdown profiles.
