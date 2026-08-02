## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2024-05-16 - Empty markdown links wrapping badges cause screen reader issues

**Learning:** Wrapping images or badges in empty markdown links (e.g.,
`[![alt](src)]()`) causes screen readers to announce them confusingly
and can cause the page to reload when clicked, leading to a poor user
experience and accessibility issues.
**Action:** Use plain image tags (`![alt](src)`) for non-interactive
badges or images instead of wrapping them in empty links to improve
screen reader accessibility and prevent unintended navigation.
