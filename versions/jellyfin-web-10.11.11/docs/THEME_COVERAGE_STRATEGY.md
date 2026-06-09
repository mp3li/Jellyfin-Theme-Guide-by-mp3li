# Theme Coverage Strategy

A good Jellyfin Web theme styles reusable components first.

Do this:

- Style cards with `.cardBox`, `.cardImage`, and `.cardText`.
- Style lists with `.listItem` and `.paperList`.
- Style forms with `.emby-input`, `.emby-select`, and `.checkboxContainer`.
- Style pages with IDs like `#loginPage` and `#itemDetailPage` only for screen-specific changes.

Avoid relying on one exact home row order. Different users can customize their home screen, so row number selectors can break easily.
