# Accessibility case note: Joplin website — keyboard focus indicator

**Target:** https://github.com/laurent22/joplin  
**Type:** Website / documentation site  
**Primary category:** Focus visibility

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** A global outline reset made some website links and controls difficult or impossible to locate during keyboard navigation.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.1.1 Keyboard, 2.4.7 Focus Visible

## Suggested / implemented fix

Remove the global outline reset and add a clear :focus-visible style for interactive controls.

## Upstream evidence

- https://github.com/laurent22/joplin/pull/15378 — merged, created 2026-05-12

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
