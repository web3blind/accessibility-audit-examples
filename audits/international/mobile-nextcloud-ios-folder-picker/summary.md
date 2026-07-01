# Nextcloud iOS — share extension folder picker

**Type:** Mobile / iOS  
**Target:** https://github.com/nextcloud/ios  
**Upstream:** https://github.com/nextcloud/ios/pull/4111

## Main issue

Folder rows in the share extension target-folder picker needed explicit VoiceOver labels and actionable semantics.

## Fix/proposal

Set accessibility labels/value text from visible folder metadata and expose folder rows as actionable elements.

## Why it matters

This is a concrete accessibility example from an upstream contribution: the visible interface behavior needed a programmatic equivalent for keyboard and/or screen-reader users.

## Status

- https://github.com/nextcloud/ios/pull/4111 — merged, created 2026-05-15
