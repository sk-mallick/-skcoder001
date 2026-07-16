## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-07-16 - Wrapping badges in empty links
**Learning:** Wrapping images or badges in empty links
(e.g., `[![alt](src)]()`) causes accessibility issues for screen readers,
as they announce the link confusingly and it reloads the page on click.
It also violates markdown linting rule MD042.
**Action:** Use plain image tags (`![alt](src)`) instead of empty links
for decorative or non-navigational badges in markdown files.
