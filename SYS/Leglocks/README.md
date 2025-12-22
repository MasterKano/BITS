# SYS / Leglocks — Canonical Systems Library

## Purpose
This folder is the *canonical* (non-duplicated) leglock systems library.
- **SYS** = “what the system is” (position, control hub, dilemma, finish mechanics)
- **INS** = “where it’s taught” (instructional, volume, chapter, timestamps)

Rule: **A concept exists once in SYS**. Instructionals add *sources* to it.

---

## De-duplication Rules (Non-Negotiable)
1. **One file per system.**  
   If another instructional teaches the same system, do *not* create a new SYS file. Add new sources to the existing file.
2. **“Different name, same system” → synonyms, not duplicates.**  
   Add alternate names inside the system file under “Synonyms / Alternate Labels”.
3. **“Same name, different system” → split and disambiguate.**  
   If two instructors use the same term differently, create separate systems with disambiguated slugs and state the difference at the top.

---

## Source Referencing Standard (How SYS links to INS)
Inside every SYS file, include a **Sources** section with bullet references using this format:

- `INS/<Instructor>/<Series>/<Instructional>/V<vol> — <Chapter Title> (start–end)`
- If you don’t know the exact chapter yet, use: `(TBD)` and update later.

Example:
- `INS/JD/ETS/Leglocks/V2 — Irimi Ashi: Entries (04:40–11:20)`

---

## System File Template (Copy into each SYS file)
Each system file should follow this structure:

1. **Definition (1–3 lines)**
2. **Scope (what is / what is not)**
3. **Entry Conditions (when it appears)**
4. **Primary Control Problems (what must be solved)**
5. **Key Mechanics / Invariants**
6. **Decision Tree (triggers → options)**
7. **Failure Modes + Fixes**
8. **Counters / Defensive Reactions**
9. **Integration Links (what systems it connects to)**
10. **Drillables (minimal viable reps)**
11. **Sources (INS references)**
12. **Synonyms / Alternate Labels**

---

## Naming + Slugs
- Slugs should be **stable and generic** (not instructor-specific).
- Prefer: `irimi-ashi-garami-entry-hub.md`
- Avoid: `danaher-irimi.md`

If a file is instructor-specific because it truly differs, prefix with a disambiguator:
- `irimi-ashi-garami-entry-hub--jd.md`
- `irimi-ashi-garami-entry-hub--ms.md`

(Only do this when the systems are materially different.)

---

## Adding a New Instructional (Procedure)
When adding a new instructional (Danaher, Gordon, Mateusz, etc.):
1. **Scan it top-down** and list the systems it contains (as candidates).
2. For each candidate:
   - If SYS file exists → add sources + any genuinely new mechanics as “Variants”.
   - If SYS file does not exist → create it using the template.
3. Never create a new SYS file when the change is only terminology.

---

## Current Instructionals to Merge (Planned)
- JD — Enter The System: Leg Locks
- GR — Systematically Attacking The Legs
- Mateusz — (to add)
- Lachlan — (later)

This README defines the rules so the library scales without duplication.
