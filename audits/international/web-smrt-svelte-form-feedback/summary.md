# smrt-svelte — form feedback relationships

**Type:** Web component library / Svelte  
**Target:** https://github.com/happyvertical/smrt  
**Upstream:** https://github.com/happyvertical/smrt/pull/1440

## Main issue

Core form primitives exposed dynamic supporting/validation text visually, but not always through a stable programmatic relationship.

## Fix/proposal

Generate stable ids, connect controls with aria-describedby, set aria-invalid and announce validation/status changes.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/happyvertical/smrt/pull/1440 — closed, created 2026-06-07
