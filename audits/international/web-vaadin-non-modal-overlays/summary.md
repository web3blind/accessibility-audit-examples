# Vaadin Web Components — non-modal overlays

**Type:** Web components / TypeScript  
**Target:** https://github.com/vaadin/web-components  
**Upstream:** https://github.com/vaadin/web-components/pull/11984

## Main issue

Non-modal dialog/popover behavior can trap keyboard focus or fail to announce useful context when an overlay opens.

## Fix/proposal

Disable focus trapping for non-modal overlays and add polite announcement behavior for popovers without moving focus unexpectedly.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/vaadin/web-components/pull/11984 — open, created 2026-06-28
