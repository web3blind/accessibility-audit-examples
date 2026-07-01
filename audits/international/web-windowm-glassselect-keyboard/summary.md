# WindoM — GlassSelect keyboard navigation

**Type:** Web app / React  
**Target:** https://github.com/YehudaBriskman/WindoM  
**Upstream:** https://github.com/YehudaBriskman/WindoM/pulls?q=author%3Aweb3blind+GlassSelect+keyboard

## Main issue

Custom GlassSelect control needed keyboard navigation, active option tracking and predictable close/select focus behavior.

## Fix/proposal

Add Arrow/Home/End/Enter/Space/Escape handling, active option state, aria-activedescendant and focus return behavior with regression tests.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/YehudaBriskman/WindoM/pull/269 — closed, created 2026-05-20
- https://github.com/YehudaBriskman/WindoM/pull/270 — open, created 2026-05-23
