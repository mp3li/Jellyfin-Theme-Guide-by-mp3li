<p align="center">
  <img src="https://raw.githubusercontent.com/jellyfin/jellyfin-ux/master/branding/SVG/icon-transparent.svg" alt="Jellyfin icon" width="72" />
</p>

<h1 align="center">Jellyfin Theme Guide by mp3li</h1>

<p align="center">
  A community documentation project for Jellyfin Web theming.
</p>

<p align="center">
  This repository documents Jellyfin Web's CSS theming surface for people who want to build custom Jellyfin themes. It is not a finished visual theme, a Jellyfin plugin, or an official Jellyfin project.
</p>

<p align="center">
  <img alt="Jellyfin Web version" src="https://img.shields.io/badge/Jellyfin_Web-10.11.11-00A4DC?style=flat-square&labelColor=101010" />
  <img alt="Selectors documented" src="https://img.shields.io/badge/selectors_documented-2%2C341-AA5CC3?style=flat-square&labelColor=101010" />
  <img alt="Guide type" src="https://img.shields.io/badge/guide-CSS_theming-00A4DC?style=flat-square&labelColor=101010" />
  <img alt="Source tag" src="https://img.shields.io/badge/source-v10.11.11-AA5CC3?style=flat-square&labelColor=101010" />
  <img alt="License" src="https://img.shields.io/badge/license-CC_BY--SA_4.0-00A4DC?style=flat-square&labelColor=101010" />
  <img alt="Project status" src="https://img.shields.io/badge/status-community_docs-AA5CC3?style=flat-square&labelColor=101010" />
</p>

## Table of Contents

<details>
<summary>Open Table of Contents</summary>

<br />

- [Current Stable Guide](#current-stable-guide)
- [What The Guide Is For](#what-the-guide-is-for)
- [Plain-English Basics](#plain-english-basics)
- [How To Read Each Entry](#how-to-read-each-entry)
- [Selector Types In Plain English](#selector-types-in-plain-english)
- [What CSS Can And Cannot Do](#what-css-can-and-cannot-do)
- [Version Scope](#version-scope)
- [How This Guide Is Organized](#how-this-guide-is-organized)
- [Category Counts](#category-counts)
- [Examples From The Guide](#examples-from-the-guide)
- [Versioned Documentation](#versioned-documentation)
- [Jellyfin Web 10.11.11 Scope](#jellyfin-web-101111-scope)
- [License and Credit](#license-and-credit)
- [Branding](#branding)

</details>

## Current Stable Guide

The current stable guide is for Jellyfin Web `10.11.11`.

- [Jellyfin Web 10.11.11 Guide](versions/jellyfin-web-10.11.11/docs/GUIDE.md)
- [Jellyfin Web 10.11.11 Directory](versions/jellyfin-web-10.11.11/docs/DIRECTORY.md)
- [Jellyfin Web 10.11.11 Dataset](versions/jellyfin-web-10.11.11/docs/theming-dataset.json)

## What The Guide Is For

The Guide is meant to be readable even if you are new to CSS theming. It explains:

- What each Jellyfin screen area is.
- What each selector is likely connected to on screen.
- What kinds of CSS properties you can usually change.
- Where the selector appears in Jellyfin Web source.
- A practical example for every documented selector.

The Directory is the same reference organized alphabetically like a glossary.

## Plain-English Basics

A **CSS selector** is the name you write before a CSS block. It tells the browser what part of the page you want to style.

Example:

```css
.cardBox {
  border-radius: 8px;
}
```

In that example, `.cardBox` is the selector. It targets Jellyfin card boxes, such as poster cards or media tiles.

## How To Read Each Entry

The full Guide and Directory are large because they document every discovered selector. Each selector entry is written in the same practical format: what it is, what kind of selector it is, where it appears in Jellyfin Web source, what CSS can usually change, and a pasteable example.

Each selector entry answers the same practical questions:

- **What it is** explains the Jellyfin screen area in normal language.
- **Selector type** explains whether the selector targets one screen, a reusable class, a built-in Jellyfin web component, an attribute, or a state like `:hover`.
- **Where it appears in source** gives the Jellyfin Web files that mention it, so advanced theme makers can inspect the original context.
- **What you can usually change** lists CSS property families that are realistic for that selector.
- **Example** gives a complete CSS block you can paste into Jellyfin's Custom CSS box and then adjust.

The examples are starting points, not rules. A selector for a page wrapper can often use background, spacing, and layout properties. A selector for a poster/card can often use radius, shadow, image sizing, and hover effects. A selector for a form control can often use border, background, focus color, height, and font styling.

## Selector Types In Plain English

- `#loginPage` starts with `#`, so it targets one specific page or unique element.
- `.cardBox` starts with `.`, so it targets a reusable class that may appear in many places.
- `emby-input` has no `.` or `#`, so it targets a custom Jellyfin web element.
- `[data-type]` targets elements that carry a specific HTML data attribute. These are useful for advanced targeting, but they can be broad.
- `.button:hover` targets a state. It applies only while the user is hovering over that element.

## What CSS Can And Cannot Do

CSS can change colors, spacing, borders, shadows, fonts, visibility, layout, hover/focus states, image fitting, and many responsive behaviors.

CSS cannot reliably add new Jellyfin features, fetch different media, change server data, rewrite page logic, or create a fully new home-screen carousel by itself. Those changes need JavaScript changes, a Jellyfin Web fork, or a plugin-level approach.

## Version Scope

- Jellyfin Web version: `10.11.11`
- Source tag: `v10.11.11`
- Source commit inspected: `35c0793ece3adbd247eab290ae1effab851f3d37`
- Stylesheet files scanned: 108
- Markup/script files scanned: 841
- Selectors documented: 2341

## How This Guide Is Organized

- The sections below match parts of the Jellyfin screen: pages, cards, lists, forms, playback, dashboard, and so on.
- Every selector has a plain-language explanation.
- Every selector has an example CSS block.
- The [Directory](versions/jellyfin-web-10.11.11/docs/DIRECTORY.md) is the same information alphabetized like a glossary.

## Category Counts

| Category | Selectors |
| --- | ---: |
| Pages and Full Screens | 62 |
| App Shell Layout and Spacing | 8 |
| Header Navigation and Tabs | 9 |
| Home Screen Rows | 6 |
| Cards Posters and Artwork | 50 |
| Lists Rows and Tables | 2 |
| Login and Server Selection | 24 |
| Libraries Search Filters and Sorting | 70 |
| Item Details and Metadata | 76 |
| Forms Inputs and Settings Controls | 188 |
| Buttons Icons and Actions | 98 |
| Dialogs Menus Toasts and Popups | 128 |
| Indicators Progress and Status | 65 |
| Playback Now Playing and OSD | 299 |
| Live TV Guide and Recording | 169 |
| Lyrics Subtitles and Text Tracks | 114 |
| Editors Uploaders and Provider Settings | 550 |
| Dashboard Admin and Users | 197 |
| Screensavers Slideshows and Swiper | 8 |
| Specialty Players and Built-in Plugins | 100 |
| Data Attribute Selectors | 98 |
| Utilities and Miscellaneous | 20 |

## Examples From The Guide

<details open>
<summary>Example: login page wrapper</summary>

<br />

`#loginPage` is the main wrapper for the Jellyfin login screen. It is useful when you want login-page-only styling without affecting the rest of Jellyfin.

```css
#loginPage {
  background: #202020;
  color: #ffffff;
  border-radius: 8px;
  padding: 0.5rem;
}
```

</details>

<details>
<summary>Example: poster and media cards</summary>

<br />

`.cardBox` is part of Jellyfin's card/artwork system. It can affect poster cards, backdrop cards, library tiles, people cards, card overlays, and fallback artwork depending on the screen.

```css
.cardBox {
  border-radius: 8px;
  box-shadow: 0 10px 24px rgba(0, 0, 0, 0.35);
  overflow: hidden;
}
```

</details>

<details>
<summary>Example: text inputs and form fields</summary>

<br />

`.emby-input` targets Jellyfin text input styling. It is useful for login fields, settings fields, dashboard forms, and other places where Jellyfin uses its standard input control.

```css
.emby-input {
  background: #151515;
  color: #ffffff;
  border: 1px solid #777777;
  border-radius: 6px;
}

.emby-input:focus {
  border-color: #00a4dc;
}
```

</details>

## Versioned Documentation

Documentation is organized by Jellyfin Web version so future versions can be added without overwriting older references.

```text
versions/
  jellyfin-web-10.11.11/
    docs/
      GUIDE.md
      DIRECTORY.md
      theming-dataset.json
      CAPABILITIES_AND_LIMITATIONS.md
      CUSTOMIZATION_GUIDE.md
      THEME_COVERAGE_STRATEGY.md
      TESTING_CHECKLIST.md
```

## Jellyfin Web 10.11.11 Scope

- Source repo: <https://github.com/jellyfin/jellyfin-web>
- Source tag: `v10.11.11`
- Source commit inspected: `35c0793ece3adbd247eab290ae1effab851f3d37`
- Jellyfin Web package version: `10.11.11`
- Stylesheet files scanned: `108`
- Markup/script files scanned: `841`
- Selectors documented: `2,341`

## License and Credit

This documentation is licensed under **Creative Commons Attribution-ShareAlike 4.0 International**.

That means people may share and adapt this work, including publicly, but they must:

- Give appropriate credit.
- Link to the license.
- Indicate if changes were made.
- Share adapted versions under the same license.

This project is based on analysis of Jellyfin Web, which is licensed `GPL-2.0-or-later`. See [ATTRIBUTION.md](ATTRIBUTION.md).

## Branding

This is an unofficial community documentation project. It is not affiliated with or endorsed by the Jellyfin project.

Official Jellyfin branding guidance:

- <https://jellyfin.org/docs/general/contributing/branding>
