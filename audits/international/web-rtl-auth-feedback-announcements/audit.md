# Accessibility case note: Ride The Lightning — auth feedback announcements

**Target:** https://github.com/Ride-The-Lightning/RTL  
**Type:** Web app / Angular  
**Primary category:** Dynamic status announcements

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Loading, validation and auth/session feedback could appear visually without being announced to screen-reader users.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 3.3.1 Error Identification, 4.1.3 Status Messages

## Suggested / implemented fix

Use live-region semantics for initial loading, assertive auth validation/login errors and polite logout/session messages.

## Upstream evidence

- https://github.com/Ride-The-Lightning/RTL/pull/1603 — open, created 2026-05-21

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
