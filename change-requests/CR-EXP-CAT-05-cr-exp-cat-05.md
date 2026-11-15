# CR-EXP-CAT-05: CR Numbering Correction (programme batch CRs)

**Status**: Landed (this PR)
**Layer**: Catalog governance (CR records)
**Owner**: Emmanuel A. Otchere
**Date**: 2026-11-15
**Trigger**: The population programme's batch admission CRs landed under numbers colliding with this series' foundation/groundwork CRs (driver numbering heuristic defect, fixed in the programme tooling). Landed CRs are immutable; corrections are recorded by later PRs (BC-01A renumbering precedent).
**Carrier**: Single PR on feature branch `feat/cr-exp-cat-05`. PR review, not direct push.
**Lands against**: `main`

## 1. What this CR does

Renames the colliding batch CR records to their next-free series numbers and updates the CR index and CHANGELOG headings:

| Landed as | Corrected to |
|---|---|
| `CR-EXP-CAT-01` | `CR-EXP-CAT-04` |

## 2. NOT-List

- No content changes to the renamed CRs; no record changes; no re-admission.
- Historical commit messages keep their original form.

## 3. Acceptance criteria

1. All mapped records exist under their corrected numbers; no number collisions remain in the series.
2. CR index and CHANGELOG reference the corrected names.
