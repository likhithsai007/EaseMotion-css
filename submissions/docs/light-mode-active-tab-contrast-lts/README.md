# Active Tab Light Mode Visibility Fix (`light-mode-active-tab-contrast-lts`)

## What does this do?
Resolves poor contrast and visibility issues for the active navigation tab (e.g. "Buttons") in the top navigation bar when switching to light mode theme.

## How is it used?
Apply theme variables to the navigation elements in the documentation stylesheet (`docs/docs.css` and `docs/demo.html`):

```css
/* Navigation link fix using theme-aware variables */
.demo-nav {
  background: var(--header-bg);
  border-bottom: 1px solid var(--border-color);
}

.demo-nav-links a {
  color: var(--nav-link-color);
}

.demo-nav-links a:hover,
.demo-nav-links a.active {
  color: var(--nav-link-active-text);
  background: var(--nav-link-active-bg);
}
```

## Why is it useful?
It aligns with EaseMotion's focus on premium aesthetics and full accessibility, ensuring that navigation elements stay clearly readable and distinguishable in both dark and light themes.
