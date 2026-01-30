PATH: META/ops/SYS-MERGE-QUEUE.md

# SYS Merge Queue — Active Run (Single Source of Truth)

## How to use (copy/paste protocol)
- This file is the **one authoritative queue** for the current SYS merge run.
- When you want me to proceed, paste:
  1) the next SYS file content (from the path listed as NEXT), and
  2) this queue file (or at minimum the “Active Queue” section).
- I must:
  - update the SYS file,
  - report Delta Summary,
  - then update this queue (status + next pointer).

## Rules (binding)
- One active queue only.
- Execute top-to-bottom.
- No jumping ahead unless you explicitly instruct.
- Each item must have exactly one status: `PENDING | MERGED | SKIPPED | DELTA`.
- “DELTA” means: merged previously, but needs audit pass at the end.

---

## Active Run Metadata
- Run ID: YYYY-MM-DD-<shortname> (you set)
- Primary scope: SYS/leglocks/
- Instructionals in scope (short tags): (fill)
- Sources available: TRN | BIO | VN (fill)

---

## Active Queue
Legend:
- Status: PENDING | MERGED | SKIPPED | DELTA
- Type: UPDATE (existing) | NEW (create)
- Notes: short reason for skip or delta

| # | Status  | Type   | PATH | Notes |
|---|---------|--------|------|-------|
| 1 | PENDING | UPDATE | SYS/leglocks/README.md | |
| 2 | PENDING | UPDATE | SYS/leglocks/ashi-hierarchy.md | |
| 3 | SKIPPED | UPDATE | SYS/leglocks/control-hubs/knee-line-and-wedge-control.md | already merged in this run |
| 4 | PENDING | UPDATE | SYS/leglocks/positions-ashi/irimi-ashi-garami-entry-hub.md | |
| 5 | PENDING | UPDATE | SYS/leglocks/transitions/post-ashi.md | |
| 6 | PENDING | UPDATE | SYS/leglocks/transitions/butterfly-ashi.md | |
| 7 | PENDING | UPDATE | SYS/leglocks/positions-ashi/outside-ashi-garami-finishing-hub.md | |
| 8 | PENDING | UPDATE | SYS/leglocks/positions-ashi/outside-ashi-garami-hip-control-outside-heel-hook-hub.md | |
| 9 | PENDING | UPDATE | SYS/leglocks/positions-ashi/cross-ashi-garami-double-trouble-platform.md | |
|10 | PENDING | UPDATE | SYS/leglocks/positions-ashi/inside-ashi-garami-outside-hh-oriented-cross-family.md | |
|11 | PENDING | UPDATE | SYS/leglocks/transitions/backside-50-50.md | |
|12 | PENDING | UPDATE | SYS/leglocks/transitions/far-hip-ashi.md | |
|13 | PENDING | UPDATE | SYS/leglocks/control-hubs/double-trouble.md | |
|14 | PENDING | UPDATE | SYS/leglocks/control-hubs/leg-lace-dracula.md | |
|15 | PENDING | UPDATE | SYS/leglocks/submissions/straight-ankle-achilles.md | |
|16 | PENDING | UPDATE | SYS/leglocks/submissions/heel-hook-system.md | |
|17 | PENDING | UPDATE | SYS/leglocks/submissions/toe-hold-system.md | |
|18 | PENDING | UPDATE | SYS/leglocks/submissions/knee-bar-system.md | |
|19 | PENDING | NEW    | SYS/leglocks/positions-ashi/50-50-hub.md | optional; decide filename |

---

## NEXT (single pointer)
- Next item number:
- Next PATH:
- Paste next: (a) SYS file content, (b) this queue (or Active Queue section)
