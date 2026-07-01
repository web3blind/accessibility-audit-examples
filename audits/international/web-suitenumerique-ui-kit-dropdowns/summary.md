# La Suite numérique UI Kit — dropdown menu semantics

**Type:** Web component library / React  
**Target:** https://github.com/suitenumerique/ui-kit  
**Upstream:** https://github.com/suitenumerique/ui-kit/pulls?q=author%3Aweb3blind+dropdown+accessibility

## Main issue

Dropdown triggers and menu items did not consistently expose expanded/open state, relationships, checked/selected state and visible keyboard focus.

## Fix/proposal

Add aria-haspopup, aria-expanded, aria-controls, stable menu ids, selected/checked semantics and clearer focus styling across several focused PRs.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/suitenumerique/ui-kit/pull/226 — closed, created 2026-05-14
- https://github.com/suitenumerique/ui-kit/pull/227 — closed, created 2026-05-15
- https://github.com/suitenumerique/ui-kit/pull/228 — closed, created 2026-05-16
- https://github.com/suitenumerique/ui-kit/pull/229 — closed, created 2026-05-17
