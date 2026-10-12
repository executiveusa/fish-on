# Fish On

Chat-first Texas fishing agent. Made in Texas, for Texans.

**Public shell:** https://executiveusa.github.io/fish-on/ — non-operational access page only. The working product is private and installed per customer.

## Product vs marketing split

This repo is the **public surface**. It holds both sides, separated by directory:

**Public shell**
- `/index.html` + `/es/` - non-operational MACS client-access pages only.
  They explain that the working product is privately installed per customer and
  point visitors back to the MACS product page.
- `/field-cards/red-drum/` (+ `/es/`) - public informational field cards:
  cited, dated regulation references anglers can read on the phone or print.
  They are not an authenticated product runtime.

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


## Access policy

The GitHub Pages site is intentionally non-operational. It must not expose a working agent, customer state, private data, or privileged API surface.

Fish On is a MACS in-house product pattern. Working deployments belong in private, customer-controlled installations with their own authentication and data boundary. The canonical private implementation is not published through this repository.
