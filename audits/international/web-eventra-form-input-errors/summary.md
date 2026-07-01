# Eventra — common form input error wiring

**Type:** Web app / React + Spring Boot  
**Target:** https://github.com/SandeepVashishtha/Eventra  
**Upstream:** https://github.com/SandeepVashishtha/Eventra/pull/4803

## Main issue

Shared FormInput labels and validation messages were not fully associated with their controls.

## Fix/proposal

Connect labels via htmlFor/id, link validation errors with aria-describedby and expose aria-invalid.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/SandeepVashishtha/Eventra/pull/4803 — open, created 2026-05-30
