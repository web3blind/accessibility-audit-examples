# Accessibility case note: PKP pkp-lib — FormHandler validation focus and error relationships

**Target:** https://github.com/pkp/pkp-lib
**Type:** Web app framework / JavaScript form controller
**Primary category:** Form validation focus and error semantics

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of OJS, OMP or OPS. The agent work focused on the shared `FormHandler` validation path and the evidence available from source code, issue context and static validation.

## Finding

- **Issue:** Failed submissions in shared PKP forms could leave keyboard and screen-reader users without a reliable programmatic path from an invalid control to its validation message.
- **Impact:** users may not land on the first invalid field after submit, may not hear the specific error associated with that field, and may receive stale or missing invalid-state information.
- **Related criteria:** 2.4.3 Focus Order, 3.3.1 Error Identification, 3.3.3 Error Suggestion, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Update the shared `FormHandler` validation behavior to move focus to the first invalid control, create stable ids for generated validation messages, preserve existing `aria-describedby` tokens, connect invalid controls to their messages, set `aria-invalid="true"` only while a control is invalid, and remove managed state when it becomes valid.

## Upstream evidence

- https://github.com/pkp/pkp-lib/pull/13031 — open, created 2026-07-12
- https://github.com/pkp/pkp-lib/issues/12635
- https://github.com/pkp/pkp-lib/issues/12599
- https://github.com/pkp/pkp-lib/issues/12837

## Validation performed

- `python3 pkp_formhandler_static_check.py`
- `node --check js/controllers/form/FormHandler.js`
- `git diff --check`

## Boundary

The agent checked available source/static evidence for this shared form-controller pattern. Runtime JAWS, NVDA, VoiceOver and application-flow verification remains a separate follow-up stage when maintainers can test in the target PKP products.
