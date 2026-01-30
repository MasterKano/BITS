# NWJJ / Open Guard 2 (OG2)

This repository contains structured working artifacts for John Danaher’s **New Wave Jiu Jitsu (NWJJ)** sub-series **Open Guard 2 (OG2)**. The goal is to convert raw instructional transcripts into a consistent, searchable, and implementation-ready knowledge base (VN → BIO → downstream deliverables).

## Repository Scope

**Series:** New Wave Jiu Jitsu (NWJJ)  
**Sub-series:** Open Guard 2 (OG2)  
**Source type:** 8-volume instructional transcripts  
**Primary outputs:**
- **VN (Viewing Notes):** per-volume “best version” operational notes (system map, ruleset, drill map, tags).
- **BIO report:** consolidated technical ontology / concept map extracted across volumes.
- (Optional downstream) technique index, decision trees, drill library, and compilation bundles.

## Structure

Recommended layout under `NWJJ/OG2/`:

NWJJ/OG2/
├─ README.md
├─ gov/                         # Governance documents for this project
├─ titles/                      # Chapter/sub-chapter titles + timecodes reference
├─ source/                      # Raw transcripts (by volume)
├─ VN/                          # Viewing Notes (VN01–VN08)
├─ BIO/                         # BIO report + supporting concept tables
└─ outputs/                     # Any compiled deliverables (indexes, drill packs, etc.)

### Key Directories

- `gov/`
  - Project governance and formatting standards used across all artifacts.
- `titles/`
  - Canonical sub-chapter titles and timecodes (used as the authoritative header text).
- `source/`
  - Volume transcripts (OG2 Vol 1–8).
- `VN/`
  - `VN01.md` … `VN08.md` (one file per volume).
- `BIO/`
  - `BIO.md` (and any appendices/tables as needed).
- `outputs/`
  - Cross-volume compilations and derivative work products.

## VN Standard (What “Best Version” Means)

Each VN file is expected to include:

1. **ASCII system diagram** (volume-level routing map)
2. **Index of sub-chapters** (exact title strings + timecodes)
3. **Global tag set** (index hooks for cross-volume compilation)
4. **Per sub-chapter notes**
   - purpose / role in the system
   - decision rules (IF/THEN)
   - non-negotiable mechanics (as applicable)
   - failure modes
   - drill hooks
5. **One-page ruleset** (non-negotiables extracted)
6. **Drill map** (rule → drill prescription with start/constraints/win/fail)
7. **Implementation summary** (minimal “keep 20%” extraction)

## Naming Conventions

- Viewing Notes: `VN01.md` … `VN08.md`
- BIO report: `BIO.md`
- Use **exact** chapter/sub-chapter title strings from the `titles/` reference in all headers.
- Timecodes should match the `titles/` file.

## Operating Principles (System-Level)

Open Guard 2 is treated as a **routing system** rather than a technique catalog:

- **Dilemmas** are the control layer (force reaction → route).
- **Knockdowns are checkpoints**, not endpoints.
- **Completion doctrine**: knockdown → **waist/behind** → consolidate.
- **Distance and posture gates** determine which hub/lane is highest probability.
- **Heist and go-behinds** are primary scoring conversions, not secondary options.

## Workflow

1. Ingest OG2 transcripts and titles file.
2. Produce `VN01–VN08` using the VN standard above.
3. Build/expand `BIO.md` by aggregating:
   - concepts, hubs, lanes, dilemmas
   - decision rules
   - failure patterns + corrections
   - drill library (cross-volume)
4. Generate any `outputs/` compilations:
   - tag-based topic bundles
   - technique index
   - training constraints and session plans

## Status

- VN: `VN01–VN08` drafted (best-version format).
- BIO: in progress / maintained as the cross-volume consolidation artifact.

## Notes

- This repo assumes prior completion of governance procedures for **Open Guard 1 (OG1)** and reuses the same operational standards unless explicitly overridden.
- Avoid adding techniques that do not improve routing or completion; dilution reduces system integrity.

---

If you want, I can also provide a shorter README variant (for a tighter GitHub front page) and a separate CONTRIBUTING.md that encodes the VN/BIO update rules and formatting checks.
