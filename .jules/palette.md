## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2024-05-16 - Removed empty link wrappers from status badges in Markdown
**Learning:** In Markdown, wrapping images in empty links (`[![alt](image.png)]()`) creates an accessibility issue where screen readers announce them as links and keyboard users can tab to them, but they are not functional and might lead to unintended behavior.
**Action:** Always ensure that status badges and other decorative images in Markdown are not wrapped in empty links. Use `![alt](image.png)` instead.
