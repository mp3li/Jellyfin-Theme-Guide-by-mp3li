# Capabilities and Limitations

This document explains what Jellyfin Web 10.11.11 Custom CSS can and cannot do.

## What CSS Can Change

CSS can change how existing Jellyfin Web elements look: colors, backgrounds, fonts, spacing, borders, shadows, card shapes, poster treatment, dialogs, forms, playback overlays, dashboard panels, and responsive layout.

## What CSS Cannot Change

CSS cannot change server behavior, API responses, metadata scanning, transcoding, authentication, permissions, database values, sort logic, or real app features. If Jellyfin does not already render an element or state, CSS cannot create a working new feature by itself.

## Why DevTools Still Helps

Everything Jellyfin Web renders comes from source code, dependencies, or runtime data. DevTools helps you see which of those documented selectors are actually present in your current page, user account, library type, and playback state.
