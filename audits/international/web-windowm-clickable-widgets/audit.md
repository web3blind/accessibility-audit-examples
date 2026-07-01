# Accessibility case note: WindoM — clickable widgets keyboard access

**Target:** https://github.com/YehudaBriskman/WindoM  
**Type:** Web app / React  
**Primary category:** Clickable custom controls

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Several clickable visual widgets were implemented in ways that reduced keyboard accessibility and state announcement clarity.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.1.1 Keyboard, 2.4.7 Focus Visible, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Convert controls to buttons where appropriate, make thumbnails keyboard-activatable and restore search engine picker state labeling.

## Upstream evidence

- https://github.com/YehudaBriskman/WindoM/pull/271 — open, created 2026-05-30

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
