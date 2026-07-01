# Accessibility case note: Vets Who Code App — form error feedback

**Target:** https://github.com/Vets-Who-Code/vets-who-code-app  
**Type:** Web app / React  
**Primary category:** Shared form validation

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Shared input and textarea validation/help text was not reliably connected to the fields for assistive technologies.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 3.3.1 Error Identification, 3.3.2 Labels or Instructions, 4.1.2 Name, Role, Value, 4.1.3 Status Messages

## Suggested / implemented fix

Add accessible ids, role=alert for error feedback, aria-describedby and aria-invalid with focused tests.

## Upstream evidence

- https://github.com/Vets-Who-Code/vets-who-code-app/pull/1120 — closed, created 2026-05-13

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
