# Accessibility recommendations draft for Культура.РФ

This is a compact message draft based on the multi-page automated audit in `audit.md`.

## Summary

The audit crawled 45 public pages across home, materials, news, live, museums, literature, architecture, afisha, cinema, music and special-project pages.

## First recommendations

1. Add exactly one meaningful `h1` on landing/category pages where the static HTML currently exposes no `h1`.
2. Review image alternatives on live/media pages: some image tags are emitted without `alt`; informative images need meaningful text, decorative images should use `alt=""` intentionally.
3. Check form controls on the homepage/search surfaces and associate them with visible labels or `aria-labelledby`.
4. Add or verify a visible-on-focus skip link to main content.
5. Avoid generic link text such as “читать” where the accessible name is unclear outside the surrounding visual context.

## Evidence

See `evidence.md` for the crawled page list and `audit.md` for examples.
