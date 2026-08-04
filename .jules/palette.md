## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2024-05-24 - Empty markdown links wrapping badges cause accessibility issues

**Learning:** Wrapping images (like badges or shields) in empty markdown links
(e.g., `[![alt](src)]()`) creates accessibility problems for screen readers,
as they announce the empty link confusingly, and clicking them often reloads
the page unexpectedly.
**Action:** Always use plain image tags (e.g., `![alt](src)`) for
non-interactive images or badges instead of wrapping them in empty links,
and remove empty links where found to improve screen reader accessibility.
