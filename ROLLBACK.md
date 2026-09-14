# Rollback record - Fish On

## 2026-09-14 consolidation (field card + GTM kit + README/claims housekeeping)

**Pre-change state:** commit `dee552c` ("Fish On landing: EN + es-MX, Texas Almanac
design, production SVG craft set", 2026-09-13T07:40:53Z).

**What this consolidation added:**
- `field-cards/red-drum/index.html` + `field-cards/red-drum/es/index.html` (new)
- `marketing/charter-ugc-kit.md` (new, from pauli-starnet creative/drafts/2026-09-14)
- `README.md` rewritten (product vs marketing split)
- `index.html` + `es/index.html`: regs-table stamp re-stamped "Checked Sep 14 2026"
  after live re-verification of all three table rows against TPWD (red drum,
  spotted seatrout, flounder); one `.regs-card` CSS rule; one field-card link under
  the regs table; one field-card link in the footer. No structural changes.

**To roll back completely:**
```bash
git revert --no-commit dee552c..HEAD && git commit -m "Revert consolidation" && git push
```
or hard: `git reset --hard dee552c && git push --force-with-lease`
GitHub Pages republishes automatically within ~1 minute of the push.

**To roll back only the landing edits** (keep the field card):
restore `index.html` and `es/index.html` from `dee552c`:
`git checkout dee552c -- index.html es/index.html && git commit -m "Restore landing" && git push`
