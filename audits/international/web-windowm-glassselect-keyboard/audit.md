# Accessibility case note: WindoM — GlassSelect keyboard navigation

**Target:** https://github.com/YehudaBriskman/WindoM  
**Type:** Web app / React  
**Primary category:** Custom select keyboard support

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Custom GlassSelect control needed keyboard navigation, active option tracking and predictable close/select focus behavior.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.1.1 Keyboard, 2.4.3 Focus Order, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Add Arrow/Home/End/Enter/Space/Escape handling, active option state, aria-activedescendant and focus return behavior with regression tests.

## Upstream evidence

- https://github.com/YehudaBriskman/WindoM/pull/269 — closed, created 2026-05-20
- https://github.com/YehudaBriskman/WindoM/pull/270 — open, created 2026-05-23

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
