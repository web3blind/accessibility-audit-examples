# Accessibility case note: La Suite numérique UI Kit — dropdown menu semantics

**Target:** https://github.com/suitenumerique/ui-kit  
**Type:** Web component library / React  
**Primary category:** Dropdown/menu semantics

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Dropdown triggers and menu items did not consistently expose expanded/open state, relationships, checked/selected state and visible keyboard focus.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.1.1 Keyboard, 2.4.7 Focus Visible, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Add aria-haspopup, aria-expanded, aria-controls, stable menu ids, selected/checked semantics and clearer focus styling across several focused PRs.

## Upstream evidence

- https://github.com/suitenumerique/ui-kit/pull/226 — closed, created 2026-05-14
- https://github.com/suitenumerique/ui-kit/pull/227 — closed, created 2026-05-15
- https://github.com/suitenumerique/ui-kit/pull/228 — closed, created 2026-05-16
- https://github.com/suitenumerique/ui-kit/pull/229 — closed, created 2026-05-17

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
