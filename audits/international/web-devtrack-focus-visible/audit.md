# Accessibility case note: DevTrack — visible focus styles

**Target:** https://github.com/Priyanshu-byte-coder/devtrack  
**Type:** Web app  
**Primary category:** Focus visibility

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Some buttons, links and controls had weak or missing visible keyboard focus indication.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 2.4.7 Focus Visible, 2.4.13 Focus Appearance

## Suggested / implemented fix

Add focus ring tokens and global :focus-visible styling with forced-colors support.

## Upstream evidence

- https://github.com/Priyanshu-byte-coder/devtrack/pull/1114 — merged, created 2026-05-25

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
