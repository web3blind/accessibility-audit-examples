# Accessibility improvement proposal for TastyTales

## Summary

Static Flutter accessibility audit found custom tap targets implemented with `GestureDetector` without matching `Semantics` wrappers, and icon-only controls that may not expose accessible names to TalkBack/VoiceOver.

## Evidence

- `lib/screens/loginScreen.dart`: tappable navigation areas use `GestureDetector`.
- `lib/screens/profileScreen.dart`: tappable profile actions use `GestureDetector`.
- `lib/screens/myrecipesScreen.dart`: recipe action uses `GestureDetector`.
- Project-wide static scan: `GestureDetector` is present, but `Semantics(` / `semanticLabel` were not found in `lib/`.

## Suggested fix

- Prefer semantic widgets (`IconButton`, `ElevatedButton`, `ListTile`) when possible.
- Where `GestureDetector` is needed, wrap the tappable area in `Semantics(label: ..., button: true, child: ...)`.
- Add `tooltip` to icon buttons or provide `Semantics` labels for icon-only controls.

## Validation

This proposal is based on an automated source accessibility audit. Manual TalkBack/VoiceOver verification can be done as a follow-up stage.
