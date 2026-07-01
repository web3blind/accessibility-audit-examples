# Accessibility case note: Artigen — action sheet focus

**Target:** https://github.com/MukundaKatta/artigen  
**Type:** Web app / React  
**Primary category:** Dialog focus management

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Action sheet/dialog opening did not reliably move accessibility focus to a meaningful title.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.4.3 Focus Order, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Move accessibility focus to the action sheet title, announce the title/fallback label and preserve modal/menu semantics.

## Upstream evidence

- https://github.com/MukundaKatta/artigen/pull/455 — closed, created 2026-05-22

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
