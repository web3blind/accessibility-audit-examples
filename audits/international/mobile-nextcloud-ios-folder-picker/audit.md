# Accessibility case note: Nextcloud iOS — share extension folder picker

**Target:** https://github.com/nextcloud/ios  
**Type:** Mobile / iOS  
**Primary category:** Mobile screen-reader labels

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Folder rows in the share extension target-folder picker needed explicit VoiceOver labels and actionable semantics.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 1.1.1 Non-text Content, 2.4.6 Headings and Labels, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Set accessibility labels/value text from visible folder metadata and expose folder rows as actionable elements.

## Upstream evidence

- https://github.com/nextcloud/ios/pull/4111 — merged, created 2026-05-15

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
