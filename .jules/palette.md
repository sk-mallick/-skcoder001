## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2024-05-15 - Empty links wrapping badges
**Learning:** Empty markdown links (`[![Alt text](image-url)]()`) are frequently used around badges, but they create accessibility issues for screen reader users and cause markdown linting violations (MD042). The screen reader reads an empty link.
**Action:** Always replace empty markdown links wrapping badges with plain image tags (`![Alt text](image-url)`).
