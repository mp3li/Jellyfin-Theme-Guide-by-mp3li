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
