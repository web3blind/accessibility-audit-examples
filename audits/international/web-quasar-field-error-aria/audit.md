# Accessibility case note: Quasar Framework — QInput/QField error semantics

**Target:** https://github.com/quasarframework/quasar  
**Type:** Web component library / Vue  
**Primary category:** Form error semantics

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Rendered field errors were visible but not programmatically connected to invalid controls.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 3.3.1 Error Identification, 3.3.3 Error Suggestion, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Add stable error ids and expose aria-invalid, aria-errormessage and aria-describedby for native QInput controls in error state.

## Upstream evidence

- https://github.com/quasarframework/quasar/pull/18323 — open, created 2026-06-14

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
