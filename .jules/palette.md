## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2024-05-19 - Removed empty links from badged images
**Learning:** Found multiple instances where status badges in the README were wrapped in empty links `[![alt](src)]()`. This is bad for accessibility because screen readers announce a link with no destination, and it causes markdown linting errors (MD042).
**Action:** Always verify that purely visual/status images in markdown profiles use plain image syntax `![alt](src)` rather than being wrapped in empty links.
