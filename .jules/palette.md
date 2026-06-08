## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2024-05-15 - Empty links wrapping badges
**Learning:** Badges wrapped in empty links `[]()` are announced as "link" by screen readers without a destination, causing confusion for users relying on assistive technologies. It also violates Markdown linting rule MD042.
**Action:** Always replace empty links wrapping badges with plain image tags `![]()` to ensure they are announced correctly as images.
