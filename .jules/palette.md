## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2024-08-06 - Empty links on decorative badges degrade accessibility

**Learning:** Wrapping decorative images or badges in empty markdown links
(e.g. `[![Badge](image)]()`) creates focusable but non-functional elements.
This disrupts keyboard navigation flow and confuses screen reader users by
announcing a link with no destination.
**Action:** Always ensure that decorative images or non-interactive badges are
implemented as simple images (e.g. `![Badge](image)`) without being wrapped in
link tags unless they have a valid destination.
