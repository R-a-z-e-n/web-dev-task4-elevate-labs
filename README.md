**Project Overview**

This small project demonstrates converting a desktop-only page into a mobile-friendly layout using CSS media queries.

**Files**
- `home.html`: example HTML page with a header, navigation, hero, a two-column intro (text + image), feature cards, and footer.
- `home.css`: site styles including desktop layout and responsive rules (media query at `max-width: 768px`).

**What I  implemented**
- Added a responsive scaffold (flexbox-based `.row` and `.col` helpers).
- Ensured images and media use `max-width: 100%` and `height: auto`.
- Added a CSS checkbox-based mobile nav toggle (`.nav-toggle`) so the menu collapses on small screens.
- Added a media query targeting `max-width: 768px` that stacks columns, reduces font sizes, tightens spacing, and prevents horizontal overflow.

**How to view locally**
1. Open the folder in your file manager and double-click `home.html`, or open it from Chrome: File → Open File... → select `home.html`.
2. Open Chrome DevTools (F12) and toggle Device Toolbar (Ctrl+Shift+M) to test mobile viewports.

Quick checklist when testing
- At widths <= 768px:
  - `.row` columns stack vertically (image appears below/above text depending on order).
  - Navigation shows the `Menu ☰` label; tap it to expand/collapse menu.
  - No horizontal scrolling or overflow; images scale to container width.
- At desktop widths:
  - Two-column layout (50% / 50%) is maintained for `.col-50`.






---
Created: November 18, 2025
