## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-07-11 - Empty links on GitHub profile badges
**Learning:** Wrapping images or badges in empty links (e.g.,
`[![alt](src)]()`) causes screen readers to announce them confusingly
and can cause page reloads upon clicking, creating an inaccessible experience.
**Action:** Use plain image tags (e.g., `![alt](src)`) for non-interactive
visual badges in markdown profiles to prevent accessibility issues
and MD042 linting errors.
