# Artigen — action sheet focus

**Type:** Web app / React  
**Target:** https://github.com/MukundaKatta/artigen  
**Upstream:** https://github.com/MukundaKatta/artigen/pull/455

## Main issue

Action sheet/dialog opening did not reliably move accessibility focus to a meaningful title.

## Fix/proposal

Move accessibility focus to the action sheet title, announce the title/fallback label and preserve modal/menu semantics.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/MukundaKatta/artigen/pull/455 — closed, created 2026-05-22
