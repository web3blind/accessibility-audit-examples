# MindTab — writing assistant live region scope

**Type:** Web app / writing assistant  
**Target:** https://github.com/AetherAssembly/MindTab  
**Upstream:** https://github.com/AetherAssembly/MindTab/pull/19

## Main issue

The whole writing assistant panel was marked as a polite live region, which could cause screen readers to announce unrelated updates while users typed.

## Fix/proposal

Scope live announcements to the suggestions container and add a regression test for the live-region markup.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/AetherAssembly/MindTab/pull/19 — closed, created 2026-05-18
