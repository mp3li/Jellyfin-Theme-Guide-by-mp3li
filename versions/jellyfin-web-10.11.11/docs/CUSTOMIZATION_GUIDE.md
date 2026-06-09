# Customization Guide

Use this workflow when making a Jellyfin Web 10.11.11 theme.

1. Open the page you want to style in Jellyfin Web.
2. Right-click the part of the page and choose Inspect.
3. Find the class or ID in DevTools.
4. Look it up in [GUIDE.md](GUIDE.md) or [DIRECTORY.md](DIRECTORY.md).
5. Try CSS live in DevTools.
6. Move working CSS into Jellyfin Dashboard > Branding > Custom CSS.

## CSS Properties You Will Use Most

- Color: `color`, `background`, `background-color`.
- Text: `font-size`, `font-weight`, `line-height`, `text-shadow`.
- Spacing: `margin`, `padding`, `gap`.
- Shape: `border`, `border-radius`, `box-shadow`.
- Layout: `display`, `width`, `max-width`, `height`, `overflow`, `position`.
- Images: `object-fit`, `background-size`, `filter`, `aspect-ratio`.

Prefer reusable selectors like `.cardBox`, `.listItem`, `.emby-input`, and `.dialog`. Use page IDs like `#loginPage` only when you want one screen to look different.
