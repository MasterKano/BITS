PATH: SYS/leglocks/README.md

# Leglocks — Systems Index (Canonical)

## Purpose

This folder is the **single canonical** systems library for leg locks in BITS.

- Canonical means: if a topic already exists in `SYS/leglocks/`, we **update that file** rather than creating a new duplicate for a new instructional.
- Detail lives in `INS/` (BIO, VN, transcripts). `SYS/` holds the durable, merged “system view.”

## Operating rules (do not break)

- **SYS is merged and canonical. INS is detailed and per-instructional.**
- If a topic fits an existing canonical page: **update the existing page**.
- Create a new canonical page **only if** the topic is truly missing and durable across instructionals.

## How to use this folder

### If you are adding a new instructional (e.g., Danaher, Gordon, Mateusz)

1. Read this index first.
2. For each concept you want to add, find the **matching canonical topic page** below.
3. Update the existing topic page (append new details, new decision rules, new failure signatures).
4. Add links in the topic page’s **Sources** section back to:
   - the instructional BIO
   - the relevant VN volume
   - (optionally) the transcript file

### If you cannot find a matching topic page

Create a new canonical topic page **only if** the topic is truly missing.

Naming rule:
- short, stable, anchor-friendly
- prefer “what it is” over “System – …”

## Formatting conventions (house style)

- Use numbered sections for systems pages (`## 1. Purpose`, `## 2. When to Use It`, etc.).
- Include an ASCII diagram where it materially improves operational use.
  - ASCII lines must be **≤130 chars**.
  - Use fenced blocks without a language label (do not use `~~~text`).
- Keep systems pages “operator-grade”: decision rules, failure signatures, completion checks, and transition targets (including top-out links where relevant).

## Canonical map (anti-duplication)

If any new instructional covers one of these, **do not create a new file**. Update the canonical page.

### A. Foundations and global strategy

- `ashi-hierarchy.md`
- `control-hubs/knee-line-and-wedge-control.md`

### B. Primary Ashi hubs (positional systems)

- `positions-ashi/irimi-ashi-garami-entry-hub.md`
- `positions-ashi/outside-ashi-garami-finishing-hub.md`
- `positions-ashi/outside-ashi-garami-hip-control-outside-heel-hook-hub.md`
- `positions-ashi/cross-ashi-garami-double-trouble-platform.md`
- `positions-ashi/inside-ashi-garami-outside-hh-oriented-cross-family.md`

### C. Connector and outcome hubs (specialized systems)

- `transitions/butterfly-ashi.md`
- `transitions/post-ashi.md`
- `transitions/far-hip-ashi.md`
- `transitions/backside-50-50.md`

### D. Two-leg control systems

- `control-hubs/double-trouble.md`
- `control-hubs/leg-lace-dracula.md`

### E. Submission systems (mechanics + dilemma use)

- `submissions/straight-ankle-achilles.md`
- `submissions/toe-hold-system.md`
- `submissions/knee-bar-system.md`
- `submissions/heel-hook-system.md`

## Open decision (recommended)

- Add a dedicated 50/50 hub page (Pillars of Defense includes a full 50/50 module).
  - Default recommendation: `positions-ashi/50-50-hub.md`

## Sources (instructional contributors)

Add to this list as you incorporate instructionals. Use relative links.

- Danaher — Enter the System: Leg Locks
  - `INS/JD/ETS/Leglocks/` (BIO/VN/transcripts)
- Gordon Ryan — Systematically Attacking the Legs
  - `INS/GR/` (BIO/VN/transcripts) (adjust to your actual folder name)
- Gordon Ryan — Pillars of Defense: Leg Locks to Back Takes
  - `INS/GR/POD/` (BIO/VN/transcripts) (adjust to your actual folder name)
- Mateusz (Szcz…)
  - `INS/<tag>/` (BIO/VN/transcripts)
