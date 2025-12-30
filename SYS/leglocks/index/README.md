PATH: SYS/Leglocks/README.md

# Leglocks — Systems Index (Canonical)

## Purpose

This folder is the **single canonical** systems library for leg locks in BITS.

- Canonical means: if a topic already exists in `SYS/Leglocks/`, we **update that file** rather than creating a duplicate for a new instructional.
- Detail lives in `INS/` (BIO, VN, transcripts). `SYS/` holds the durable, merged “system view.”

## How to use this folder

### If you are adding a new instructional (e.g., Danaher, Gordon, Mateusz)

1. Use the **Canonical map (current pages)** below to find the closest matching system page.
2. Update that existing system page (append new rules, branches, failure signatures, constraints).
3. Add links in that system page’s **Sources** section back to:
   - the instructional BIO
   - the relevant VN volume(s)
   - (optionally) transcript file(s)

### If you cannot find a matching page

Create a new canonical topic page **only if** the topic is genuinely missing.

Naming rule:
- short, stable, anchor-friendly
- prefer “what it is” over “System – …”
- kebab-case filenames

## Canonical map (current pages)

These files currently exist in `SYS/Leglocks/`. If a new instructional covers any of these, **do not create a new file**—update the relevant one.

### A) Foundations (global constraints and maps)

- `ashi-hierarchy.md`
  - Taxonomy / hierarchy map across major Ashi families; what each hub is for; how to move between hubs.
- `knee-line-and-wedge-control.md`
  - Knee-line gates, hip line, wedges, structure-first rules; “no knee line, no break.”

### B) Primary hubs and connectors (positional systems)

- `irimi-ashi-garami-entry-hub.md`
  - Default structured entry hub; stabilise knee line; upgrade pathways.
- `outside-ashi-garami-finishing-hub.md`
  - Outside Ashi as primary asymmetrical finishing hub.
- `outside-ashi-garami-hip-control-outside-heel-hook-hub.md`
  - Outside Ashi variant emphasis (hip control + outside HH).  
  - **NOTE:** likely overlaps with the finishing hub file; treat as “candidate-to-merge” (see below).
- `cross-ashi-garami-double-trouble-platform.md`
  - Cross Ashi as high-offence hub + two-leg control platform (Double Trouble integration).
- `inside-ashi-garami-outside-hh-oriented-cross-family.md`
  - Inside Ashi (cross-family variant) oriented to outside HH lines.
- `butterfly-ashi.md`
  - Connector hub for mobility, re-angling, and preserving knee line under pressure.
- `post-ashi.md`
  - Reaction hub for posting/standing/forward drive; post-as-wedge logic.
- `backside-50-50.md`
  - Offensive resolution hub for rolls / 50-50-like exchanges; asymmetry upgrade.
- `far-hip-ashi.md`
  - Safety shell + asymmetry rebuild; foot-hiding discipline.

### C) Two-leg control systems

- `double-trouble.md`
  - Two-leg control hub; immobilisation goals; dilemma pairing logic.
- `leg-lace-dracula.md`
  - Leg lace / Dracula immobilisation structures; systematic exposure logic.

### D) Submission systems (mechanics + dilemma use)

- `straight-ankle-achilles.md`
- `toe-hold-system.md`
- `knee-bar-system.md`
- `heel-hook-system.md`

## Consolidation backlog (avoid long-term duplication)

These are *not new files to create*. They are candidates to **merge** to keep SYS canonical.

- **Outside Ashi duplication risk**
  - `outside-ashi-garami-finishing-hub.md`
  - `outside-ashi-garami-hip-control-outside-heel-hook-hub.md`
  - Expected outcome: 1 canonical Outside Ashi page with subsections (Hip Control, Heel Exposure, High-Leg responses, Roll-following, Dilemmas).

## Planned canonical pages (create only when needed)

These pages do **not** currently exist. Create only if/when you actually need them and there is no suitable existing page.

- `50-50.md`
- `mutual-ashi.md`
- `top-ushiro.md`
- `entry-principles.md`
- `asymmetry-vs-symmetry.md`
- `decision-trees.md`
- `common-failures-and-fixes.md`
- `drills-and-games.md`

## Sources (instructional contributors)

Add to this list as you incorporate instructionals. Use relative links.

- Danaher — Enter the System: Leg Locks
  - `INS/JD/ETS/Leglocks/`
- Gordon Ryan — Systematically Attacking the Legs
  - `INS/GR/...` (update to your actual folder)
- Mateusz (Szcz…)
  - `INS/<tag>/` (update to your actual folder)

## Operating rule (do not break)

- **SYS is merged and canonical. INS is detailed and per-instructional.**
- If you find yourself creating “Danaher version” and “Gordon version” of the same system page inside `SYS/Leglocks/`, stop and merge into the canonical page instead.