## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2026-05-17 - Empty Link Wrappers on Images in READMEs
**Learning:** This repository extensively used empty markdown links (e.g., `[![Badge](url)]()`) around status badges and images to perhaps inherit styling, but this creates significant accessibility issues. Empty links act as meaningless tab stops for keyboard users and cause screen readers to announce a link without a destination.
**Action:** When working on markdown documentation profiles, proactively search for and remove empty `[]()` wrappers around images to ensure a streamlined screen reader and keyboard navigation experience.
