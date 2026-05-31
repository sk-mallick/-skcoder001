## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-05-31 - Avoid empty markdown links around badges
**Learning:** Wrapping images or badges in empty markdown links (e.g., `[![alt](src)]()`) can cause accessibility issues for screen readers and violate markdown linting rules (MD042). Screen readers may try to announce the link destination, causing confusion when it is empty.
**Action:** Use plain image tags (`![alt](src)`) instead of empty links for static badges and images.
