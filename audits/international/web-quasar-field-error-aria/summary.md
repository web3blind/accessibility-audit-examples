# Quasar Framework — QInput/QField error semantics

**Type:** Web component library / Vue  
**Target:** https://github.com/quasarframework/quasar  
**Upstream:** https://github.com/quasarframework/quasar/pull/18323

## Main issue

Rendered field errors were visible but not programmatically connected to invalid controls.

## Fix/proposal

Add stable error ids and expose aria-invalid, aria-errormessage and aria-describedby for native QInput controls in error state.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/quasarframework/quasar/pull/18323 — open, created 2026-06-14
