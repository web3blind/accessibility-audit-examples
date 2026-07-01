# Accessibility case note: Eventra — common form input error wiring

**Target:** https://github.com/SandeepVashishtha/Eventra  
**Type:** Web app / React + Spring Boot  
**Primary category:** Shared form components

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Shared FormInput labels and validation messages were not fully associated with their controls.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 1.3.1 Info and Relationships, 3.3.1 Error Identification, 3.3.2 Labels or Instructions, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Connect labels via htmlFor/id, link validation errors with aria-describedby and expose aria-invalid.

## Upstream evidence

- https://github.com/SandeepVashishtha/Eventra/pull/4803 — open, created 2026-05-30

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
