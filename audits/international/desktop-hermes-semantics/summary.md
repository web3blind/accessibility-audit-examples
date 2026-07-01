# Hermes Desktop — accessibility semantics

**Type:** Desktop / Electron-like React surfaces  
**Target:** https://github.com/NousResearch/hermes-agent  
**Upstream:** https://github.com/NousResearch/hermes-agent/pull/49413

## Main issue

Desktop chat surfaces had repeated semantic gaps around autocomplete popovers, dialogs and controls.

## Fix/proposal

Add ARIA combobox/listbox relationships, improve dialog/control semantics, and document the static audit findings.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/NousResearch/hermes-agent/pull/49413 — open, created 2026-06-20
