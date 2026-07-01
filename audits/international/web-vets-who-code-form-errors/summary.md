# Vets Who Code App — form error feedback

**Type:** Web app / React  
**Target:** https://github.com/Vets-Who-Code/vets-who-code-app  
**Upstream:** https://github.com/Vets-Who-Code/vets-who-code-app/pull/1120

## Main issue

Shared input and textarea validation/help text was not reliably connected to the fields for assistive technologies.

## Fix/proposal

Add accessible ids, role=alert for error feedback, aria-describedby and aria-invalid with focused tests.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/Vets-Who-Code/vets-who-code-app/pull/1120 — closed, created 2026-05-13
