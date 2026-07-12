# PKP pkp-lib — FormHandler validation focus and error relationships

**Type:** Web app framework / JavaScript form controller
**Target:** https://github.com/pkp/pkp-lib
**Upstream:** https://github.com/pkp/pkp-lib/pull/13031

## Main issue

Failed submissions in shared PKP forms could leave keyboard and screen-reader users without a reliable programmatic path from the invalid control to the validation message.

## Fix/proposal

Move focus to the first invalid control, give generated validation messages stable ids, preserve existing `aria-describedby`, wire invalid controls to their message, and clean up managed invalid state when a field becomes valid.

## Why it matters

This is a shared layer used by OJS/OMP form flows. Fixing the common validation path can improve multiple submission and registration experiences instead of patching a single screen.

## Status

- https://github.com/pkp/pkp-lib/pull/13031 — open, created 2026-07-12
- Related issues: https://github.com/pkp/pkp-lib/issues/12635, https://github.com/pkp/pkp-lib/issues/12599, https://github.com/pkp/pkp-lib/issues/12837
