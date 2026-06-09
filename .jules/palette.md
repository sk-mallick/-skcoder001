## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2024-06-09 - Empty Links on GitHub Profile Badges
**Learning:** Adding empty markdown links `[]()` around badges or images creates accessibility issues. Screen readers announce the empty link, which provides no context and degrades the experience. It also triggers `markdownlint` MD042 errors.
**Action:** Always use plain image tags `![alt](src)` without wrapping them in empty links `[]()` when the image doesn't need to be interactive, improving both accessibility and linting compliance.
