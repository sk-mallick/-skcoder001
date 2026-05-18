## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2024-05-16 - Empty links wrapping static badges
**Learning:** Wrapping static elements like status badges in empty links (`[]()`) creates an accessibility and interaction anti-pattern in markdown where the element appears focusable and clickable but leads nowhere.
**Action:** Avoid wrapping unclickable images or badges in empty links.
