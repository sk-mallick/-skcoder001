## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-07-08 - Accessibility of Badges in GitHub Profiles
**Learning:** Wrapping images or badges in empty links
(e.g., `[![<alt>](<src>)]()`) causes screen readers to announce them
confusingly and can reload the page on click, leading to poor
accessibility and markdown linting errors (MD042).
**Action:** Use plain image tags (e.g., `![<alt>](<src>)`)
instead of empty links for static badges or images.
