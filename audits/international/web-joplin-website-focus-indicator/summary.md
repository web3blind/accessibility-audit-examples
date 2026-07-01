# Joplin website — keyboard focus indicator

**Type:** Website / documentation site  
**Target:** https://github.com/laurent22/joplin  
**Upstream:** https://github.com/laurent22/joplin/pull/15378

## Main issue

A global outline reset made some website links and controls difficult or impossible to locate during keyboard navigation.

## Fix/proposal

Remove the global outline reset and add a clear :focus-visible style for interactive controls.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/laurent22/joplin/pull/15378 — merged, created 2026-05-12
