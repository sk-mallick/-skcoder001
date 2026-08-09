## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2024-05-24 - Empty markdown links on badges
**Learning:** Using `[![alt](url)]()` to render badges in Markdown creates focusable, empty anchor links (`<a href="">`), which is an accessibility anti-pattern. This often happens when developers copy badge markup that assumes it should link somewhere, but leave the URL empty.
**Action:** When adding static visual badges or tags, always use standard image syntax `![alt](url)` instead of link-wrapped image syntax with an empty URL.
