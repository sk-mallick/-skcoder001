## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2024-05-20 - Empty links around markdown images
**Learning:** Wrapping images or badges in empty links (e.g., `[![<alt>](<src>)]()`) creates accessibility issues. Screen readers encounter an interactive element (the link) that goes nowhere, leading to confusion. This also violates markdown linting rule MD042.
**Action:** Use plain image tags (`![<alt>](<src>)`) when you only want to display an image and not link it anywhere.
