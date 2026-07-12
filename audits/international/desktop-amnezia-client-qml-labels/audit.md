# Accessibility case note: Amnezia Client — QML accessible labels

**Target:** https://github.com/amnezia-vpn/amnezia-client  
**Type:** Desktop/mobile / Qt Quick QML  
**Primary category:** Screen-reader names / QML controls

## Scope

This public example documents a real upstream accessibility contribution by `web3blind`. It is not presented as a full manual screen-reader certification of the whole product. The agent work focused on the affected component/pattern and the evidence available from source code, issue context and static review.

## Finding

- **Issue:** Core QML controls and icon-only actions could be unnamed or unclear for NVDA/TalkBack users; issue #2778 also documents core-screen and split-tunneling interaction problems.
- **Impact:** keyboard and/or assistive-technology users may miss state, labels, errors, status changes or reachable controls that are visually apparent.
- **Related criteria:** 1.1.1 Non-text Content, 2.4.6 Headings and Labels, 4.1.2 Name, Role, Value

## Suggested / implemented fix

Add Accessible.name and Accessible.role metadata to shared buttons, tabs, radio buttons, checkboxes, switchers, dropdowns, label buttons and text fields.

## Upstream evidence

- https://github.com/amnezia-vpn/amnezia-client/issues/2778 — issue covering NVDA/TalkBack problems in core controls and split tunneling
- https://github.com/amnezia-vpn/amnezia-client/pull/2779 — open, created 2026-06-27

## Boundary

The agent checked available source/static evidence for this component or pattern. Runtime screen-reader and device verification remains a separate follow-up stage when maintainers can test in the target environment.
