# Accessibility case note: IBM MCP Context Forge — admin UI modal and validation semantics

**Target:** https://github.com/IBM/mcp-context-forge  
**Type:** Web app / Admin UI  
**Primary category:** Modals / form validation

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Shared admin UI modal helpers and form validation patterns were visually available but not reliably exposed through dialog semantics and field-error relationships.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.1.1 Keyboard, 2.4.3 Focus Order, 3.3.1 Error Identification, 3.3.2 Labels or Instructions, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Add dialog labeling/focus behavior and connect invalid fields to visible validation messages with aria-invalid and aria-describedby.

## Upstream evidence

- https://github.com/IBM/mcp-context-forge/pull/5331 — open, created 2026-06-21

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
