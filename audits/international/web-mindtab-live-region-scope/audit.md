# Accessibility case note: MindTab — writing assistant live region scope

**Target:** https://github.com/AetherAssembly/MindTab  
**Type:** Web app / writing assistant  
**Primary category:** Live region noise

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** The whole writing assistant panel was marked as a polite live region, which could cause screen readers to announce unrelated updates while users typed.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 4.1.3 Status Messages

## Suggested / implemented fix

Scope live announcements to the suggestions container and add a regression test for the live-region markup.

## Upstream evidence

- https://github.com/AetherAssembly/MindTab/pull/19 — closed, created 2026-05-18

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
