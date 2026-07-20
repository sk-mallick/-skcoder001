## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2026-07-20 - Empty links around badges cause a11y issues

**Learning:** Wrapping image badges in empty links (e.g., `[![alt](src)]()`) creates accessibility issues for screen readers. They announce them confusingly and can cause page reloads if accidentally clicked. It also triggers markdown linting errors (MD042).
**Action:** Avoid wrapping badges or images in empty links in markdown files. Use plain image tags (`![alt](src)`) instead unless they are meant to navigate to a specific URL.
