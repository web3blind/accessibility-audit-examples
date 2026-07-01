# Ride The Lightning — auth feedback announcements

**Type:** Web app / Angular  
**Target:** https://github.com/Ride-The-Lightning/RTL  
**Upstream:** https://github.com/Ride-The-Lightning/RTL/pull/1603

## Main issue

Loading, validation and auth/session feedback could appear visually without being announced to screen-reader users.

## Fix/proposal

Use live-region semantics for initial loading, assertive auth validation/login errors and polite logout/session messages.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/Ride-The-Lightning/RTL/pull/1603 — open, created 2026-05-21
