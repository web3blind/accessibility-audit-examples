# Accessibility case note: smrt-svelte — form feedback relationships

**Target:** https://github.com/happyvertical/smrt  
**Type:** Web component library / Svelte  
**Primary category:** Form primitives

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Core form primitives exposed dynamic supporting/validation text visually, but not always through a stable programmatic relationship.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 3.3.1 Error Identification, 3.3.2 Labels or Instructions, 4.1.2 Name, Role, Value, 4.1.3 Status Messages

## Suggested / implemented fix

Generate stable ids, connect controls with aria-describedby, set aria-invalid and announce validation/status changes.

## Upstream evidence

- https://github.com/happyvertical/smrt/pull/1440 — closed, created 2026-06-07

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
