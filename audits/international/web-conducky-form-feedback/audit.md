# Accessibility case note: Conducky — form feedback announcements

**Target:** https://github.com/mattstratton/conducky  
**Type:** Web app  
**Primary category:** Form feedback announcements

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Visible form validation/server feedback could appear without an announcement path for assistive technologies.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 3.3.1 Error Identification, 4.1.3 Status Messages

## Suggested / implemented fix

Add alert/status roles for validation, registration error and success feedback.

## Upstream evidence

- https://github.com/mattstratton/conducky/pull/459 — open, created 2026-05-28

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
