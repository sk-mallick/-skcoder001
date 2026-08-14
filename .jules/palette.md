## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2024-05-24 - Empty markdown links create accessibility dead stops

**Learning:** Wrapping image badges in empty markdown links
(e.g. `[![alt](url)]()`) creates focusable anchor elements without a
destination. This negatively impacts accessibility by introducing dead stops
for keyboard navigation and screen readers.

**Action:** When adding static badges, use standard image syntax
(e.g. `![alt](url)`) rather than link syntax, unless the badge is intended
to link to a valid URL.
