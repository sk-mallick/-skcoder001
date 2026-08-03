## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2024-05-16 - Empty links on profile badges
**Learning:** Wrapping images (like status badges) in empty markdown links (e.g., `[![alt](src)]()`) causes accessibility issues, as screen readers announce the link confusingly and clicks reload the page.
**Action:** Use plain image tags (`![alt](src)`) instead of wrapping them in empty links.
