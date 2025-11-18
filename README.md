**Project Overview**

This small project demonstrates converting a desktop-only page into a mobile-friendly layout using CSS media queries.

**Files**
- `home.html`: example HTML page with a header, navigation, hero, a two-column intro (text + image), feature cards, and footer.
- `home.css`: site styles including desktop layout and responsive rules (media query at `max-width: 768px`).

**What I changed / implemented**
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

**Customizing / Where to edit**
- Change breakpoint: edit the `@media (max-width: 768px)` block in `home.css` to your desired breakpoint.
- Adjust container max width: edit `.container { max-width: 1200px; }` in `home.css`.
- Replace the placeholder image in `home.html` with your own asset; keep the `img` tag so responsive rules apply.
- If you prefer a JS-based nav toggle (for animation or aria improvements), replace the checkbox pattern with a small script and add appropriate `aria-*` attributes.

**Accessibility notes**
- The checkbox toggle is keyboard operable, but you may want to add `aria-expanded` and `aria-controls` when using a JS toggle for better screen reader support.
- Focus outlines are preserved with a visible focus style in `home.css`.

**Next steps (optional)**
- Add transitions/animations for the nav menu opening/closing (CSS or JS).
- Convert layout to CSS Grid for more complex responsive arrangements.
- Add more breakpoints (tablet/large desktop) for finer control.
- Run Lighthouse in Chrome for automated accessibility and performance suggestions.

If you'd like, I can:
- Replace the checkbox nav with a small accessible JS toggle (I can add the script and ARIA attributes), or
- Tune spacing and typography to match an existing brand/style — tell me the design and I will update `home.css`.

---
Created: November 18, 2025
