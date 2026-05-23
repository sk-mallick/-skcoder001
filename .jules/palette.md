## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2024-05-16 - Empty links wrapping badges cause a11y issues
**Learning:** Using `[![alt](src)]()` empty links to wrap badges creates poor UX and accessibility issues. Screen readers announce an empty link which confuses users, and clicking it causes a redundant page refresh.
**Action:** When displaying badges or images that don't need a destination, use plain image tags `![alt](src)` instead of empty link wrappers.
