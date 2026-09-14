# Fish On

Chat-first Texas fishing agent. Made in Texas, for Texans.

**Live:** https://executiveusa.github.io/fish-on/ (es-MX: https://executiveusa.github.io/fish-on/es/)

## Product vs marketing split

This repo is the **public surface**. It holds both sides, separated by directory:

**Product** (what an angler uses)
- `/index.html` + `/es/` - the chat-first landing. The chat composer is an
  **agent preview**: sample answers from real Texas sources, labeled as such on
  the page. The live agent backend is being built in `executiveusa/fish-on-texas`
  (private build lane); until it ships, every chat surface here stays labeled preview.
- `/field-cards/red-drum/` (+ `/es/`) - pocket field cards: cited, dated
  regulation cards anglers can read on the phone or print. First card: red drum.

**Marketing** (what sells the product)
- The landing itself (Bar B skeleton, Texas Almanac design, gauntlet-passed).
- `/marketing/charter-ugc-kit.md` - GTM asset for the charter/guide lane:
  five claims-safe 9:16 ad concepts plus a charter landing template. Production
  runs through Buffer Blaster; no renders until a real charter client signs.

## Claims discipline (hard rules, enforced in review)

- Every regulation number on a page carries its TPWD source link and a
  "Checked <date>" stamp. Re-verify against the live TPWD page before touching it.
- No catch-rate, success-rate, or "guaranteed fish" language anywhere.
- No specific fishing spots named (no spot-burning).
- EN first, es-MX second, visible switcher + hreflang.
- Footer always carries: TPWD non-affiliation, regulations-change disclaimer.

## Sources

TPWD Outdoor Annual (regulations, stocking) - NWS (weather) - NOAA CO-OPS (tides) - USGS (flows).

## Rollback

See `ROLLBACK.md`. Pre-consolidation state is commit `dee552c`.
