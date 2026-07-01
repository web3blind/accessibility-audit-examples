# WindoM — clickable widgets keyboard access

**Type:** Web app / React  
**Target:** https://github.com/YehudaBriskman/WindoM  
**Upstream:** https://github.com/YehudaBriskman/WindoM/pull/271

## Main issue

Several clickable visual widgets were implemented in ways that reduced keyboard accessibility and state announcement clarity.

## Fix/proposal

Convert controls to buttons where appropriate, make thumbnails keyboard-activatable and restore search engine picker state labeling.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/YehudaBriskman/WindoM/pull/271 — open, created 2026-05-30
