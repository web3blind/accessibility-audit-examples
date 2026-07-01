# IBM MCP Context Forge — admin UI modal and validation semantics

**Type:** Web app / Admin UI  
**Target:** https://github.com/IBM/mcp-context-forge  
**Upstream:** https://github.com/IBM/mcp-context-forge/pull/5331

## Main issue

Shared admin UI modal helpers and form validation patterns were visually available but not reliably exposed through dialog semantics and field-error relationships.

## Fix/proposal

Add dialog labeling/focus behavior and connect invalid fields to visible validation messages with aria-invalid and aria-describedby.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/IBM/mcp-context-forge/pull/5331 — open, created 2026-06-21
