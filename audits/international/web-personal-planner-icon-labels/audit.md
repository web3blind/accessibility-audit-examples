# Accessibility case note: Personal Planner — icon-only control labels

**Target:** https://github.com/TemaDeveloper/personal_planner  
**Type:** Web app  
**Primary category:** Accessible names / toggle state

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Icon-only, emoji, color-swatch and filled-square controls could be unnamed or unclear for screen-reader users.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 1.1.1 Non-text Content, 2.4.6 Headings and Labels, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Add accessible names to visual-only controls and aria-pressed to toggle-like buttons.

## Upstream evidence

- https://github.com/TemaDeveloper/personal_planner/pull/28 — merged, created 2026-05-19

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
