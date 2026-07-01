# La Suite numérique Docs — export select focus stop

**Type:** Web app / document editor  
**Target:** https://github.com/suitenumerique/docs  
**Upstream:** https://github.com/suitenumerique/docs/pull/2366

## Main issue

A decorative export-format select arrow was reachable as a separate keyboard/screen-reader focus stop.

## Fix/proposal

Remove the decorative arrow from tab order and hide it from assistive technologies.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/suitenumerique/docs/pull/2366 — closed, created 2026-05-29
