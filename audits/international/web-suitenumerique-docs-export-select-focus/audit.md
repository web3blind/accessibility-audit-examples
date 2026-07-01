# Accessibility case note: La Suite numérique Docs — export select focus stop

**Target:** https://github.com/suitenumerique/docs  
**Type:** Web app / document editor  
**Primary category:** Keyboard focus noise

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** A decorative export-format select arrow was reachable as a separate keyboard/screen-reader focus stop.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.1.1 Keyboard, 2.4.3 Focus Order, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Remove the decorative arrow from tab order and hide it from assistive technologies.

## Upstream evidence

- https://github.com/suitenumerique/docs/pull/2366 — closed, created 2026-05-29

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
