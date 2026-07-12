# Amnezia Client — QML accessible labels

**Type:** Desktop/mobile / Qt Quick QML  
**Target:** https://github.com/amnezia-vpn/amnezia-client  
**Upstream:** https://github.com/amnezia-vpn/amnezia-client/pull/2779

## Main issue

Core QML controls and icon-only actions could be unnamed or unclear for NVDA/TalkBack users. Issue #2778 also documents core-screen and split-tunneling interaction problems: server selection, neighboring action buttons, tabs, delete actions, search-field behavior and checkbox activation.

## Fix/proposal

Add Accessible.name and Accessible.role metadata to shared buttons, tabs, radio buttons, checkboxes, switchers, dropdowns, label buttons and text fields.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/amnezia-vpn/amnezia-client/issues/2778
- https://github.com/amnezia-vpn/amnezia-client/pull/2779 — open, created 2026-06-27
