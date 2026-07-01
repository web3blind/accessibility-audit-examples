# Accessibility case note: Drinkup — form control accessibility

**Target:** https://github.com/johnnymackcodes/drinkup  
**Type:** Web app  
**Primary category:** Form controls / status feedback

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Range/number controls, preset choices, decorative emoji and share-copy feedback needed better accessible names, state and status announcements.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 1.1.1 Non-text Content, 2.1.1 Keyboard, 4.1.2 Name, Role, Value, 4.1.3 Status Messages

## Suggested / implemented fix

Add accessible names/value text, expose choices as radio groups with keyboard support, hide decorative emoji and announce copied share links politely.

## Upstream evidence

- https://github.com/johnnymackcodes/drinkup/pull/7 — closed, created 2026-05-24

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
