## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-06-24 - Avoid empty links on badges
**Learning:** Wrapping images or badges in empty links
(e.g., `[![<alt>](<src>)]()`) causes accessibility issues for
screen readers. They announce the empty link confusingly and
can reload the page on click. It also violates markdownlint
MD042.
**Action:** Avoid wrapping images or badges in empty links.
Use plain image tags instead (`![<alt>](<src>)`).
