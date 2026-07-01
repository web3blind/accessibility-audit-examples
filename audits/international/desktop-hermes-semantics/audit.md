# Accessibility case note: Hermes Desktop — accessibility semantics

**Target:** https://github.com/NousResearch/hermes-agent  
**Type:** Desktop / Electron-like React surfaces  
**Primary category:** Desktop UI semantics

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Desktop chat surfaces had repeated semantic gaps around autocomplete popovers, dialogs and controls.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.1.1 Keyboard, 2.4.3 Focus Order, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Add ARIA combobox/listbox relationships, improve dialog/control semantics, and document the static audit findings.

## Upstream evidence

- https://github.com/NousResearch/hermes-agent/pull/49413 — open, created 2026-06-20

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
