# Accessibility case note: Vaadin Web Components — non-modal overlays

**Target:** https://github.com/vaadin/web-components  
**Type:** Web components / TypeScript  
**Primary category:** Focus management / status announcement

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Non-modal dialog/popover behavior can trap keyboard focus or fail to announce useful context when an overlay opens.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.1.1 Keyboard, 2.1.2 No Keyboard Trap, 2.4.3 Focus Order, 4.1.3 Status Messages

## Suggested / implemented fix

Disable focus trapping for non-modal overlays and add polite announcement behavior for popovers without moving focus unexpectedly.

## Upstream evidence

- https://github.com/vaadin/web-components/pull/11984 — open, created 2026-06-28

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
