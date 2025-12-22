# SYS/Leglocks — System Registry (Canonical)

## Purpose
This folder contains the **canonical** leg-lock systems for BITS.  
Rule: **One concept = one system file**. New instructionals do not create new systems unless the concept is genuinely new; they extend existing systems via **Sources + Deltas**.

## Operating Rules (No Duplication)
1. **Canonical-first**: Before creating a new system file, search this folder for an existing match (including aliases).
2. **One file per system**: If Danaher + Gordon + Mateusz cover the same system, they all live in the same system file under **Sources**.
3. **Instructionals never define systems**: `INS/...` holds viewing notes and “what the instructor said/did.”  
   `SYS/...` holds the consolidated, instructor-agnostic system.
4. **New info policy**: When a new instructor adds value, record it as a **Delta** (what is different / better / unique) rather than rewriting the whole system.

## System File Standard (Required)
Each `SYS/Leglocks/<system>.md` must contain:
- `# <System Name>`
- `## Scope`
- `## Preconditions`
- `## Core Structure`
- `## Primary Attacks`
- `## Primary Defences + Counters`
- `## Transitions (Inputs/Outputs)`
- `## Failure Modes`
- `## Drills`
- `## Sources (Instructional Cross-Refs)`
- `## Deltas by Instructor (What’s unique)`

### Sources Format (use this exact pattern)
In every system file, the **Sources** section must include entries like:
- `INS:<slug> | Vol X | Chapter: <name> | Time: 00:00–00:00 | Note: <why it matters>`

This keeps systems consolidated while preserving a fast path back to the video.

## Canonical Systems List (Leglocks)
> Update filenames to kebab-case and ensure `.md` extension over time.  
> This list is the source of truth for what exists.

1. Ashi Garami Hierarchy and Family Map → `ashi-garami-hierarchy-family-map.md`
2. Knee Line and Wedge Control → `knee-line-and-wedge-control.md`
3. Irimi Ashi Garami (Entry Hub) → `irimi-ashi-garami-entry-hub.md`
4. Outside Ashi Garami (Finishing Hub) → `outside-ashi-garami-finishing-hub.md`
5. Outside Ashi: Hip Control (Outside HH Hub) → `outside-ashi-garami-hip-control-outside-heel-hook-hub.md`
6. Cross Ashi: Double Trouble Platform → `cross-ashi-garami-double-trouble-platform.md`
7. Inside Ashi (Outside-HH Oriented Cross Family) → `inside-ashi-garami-outside-hh-oriented-cross-family.md`
8. Backside 50/50 → `backside-50-50.md`
9. Far-Hip Ashi → `far-hip-ashi.md`
10. Butterfly Ashi (Connector Hub) → `butterfly-ashi.md`
11. Post Ashi (Standing/Posting Reaction Hub) → `post-ashi.md`
12. Top Ushiro (Top Control Outcome Hub) → `top-ushiro.md`
13. Double Trouble (Two-Leg Control Hub) → `double-trouble.md`
14. Leg Lace / Dracula Controls → `leg-lace-dracula.md`
15. Straight Ankle (Achilles) System → `straight-ankle-achilles.md`
16. Toe Hold System → `toe-hold-system.md`
17. Knee Bar System → `knee-bar-system.md`
18. Heel Hook System → `heel-hook-system.md`

## Backlog (Housekeeping — do later)
- Eliminate duplicates (same concept, different filenames).
- Standardise naming: lowercase kebab-case + `.md` only.
- Ensure every system file has the required sections and “Sources + Deltas”.
