## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-06-20 - Empty links wrapping images cause accessibility issues
**Learning:** Wrapping images or badges in empty links (e.g., `[![<alt>](<src>)]()`) causes accessibility issues for screen readers. They announce them confusingly and can cause the page to reload when clicked, leading to a poor user experience. This pattern also violates markdownlint rule MD042.
**Action:** Use plain image tags (e.g., `![<alt>](<src>)`) for displaying images or badges unless they are intended to link to a valid, meaningful destination.
