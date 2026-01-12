PATH: Kano-Scroll.md

# Kano Scroll v4.0 — BITS Training Guidance Manual (PUBLISHED)

## 0. Purpose

- Provide a repeatable method to learn and train from grappling instructionals using:
  - `INS/` — per-instructional workspace (VN + sessions + source artifacts)
  - `SYS/` — one unified, deduplicated systems library
- Enforce provenance for anything promoted into `SYS/`:
  - [I] raw transcript (source-of-truth) and/or
  - [B] BIO report generated from transcript
  - VN is allowed as an intermediate operator note layer, but SYS claims must remain traceable to I/B.
- Separate manuals, separate scopes:
  - **Kano Scroll** = repo structure, naming/numbering, VN/session standards, SYS promotion workflow, startup protocol.
  - **Jigoro Text** = BIO generation rules, locked BIO template, and batch/chunk delivery grammar.
  - **BOA-SYS** = SYS merge operating agreement (queue discipline + delta reporting).

---

## 1. Repository Layout (Canonical)

### 1.1 Root

- `INS/` — Instructionals (one folder per instructional)
- `SYS/` — Systems library (canonical, merged, deduped)
- `TEMPLATES/` — copy/paste templates (VN, sessions, SYS skeletons)
- `META/` — indexes + conventions + operational notes (recommended)

### 1.2 INS Folder Standard

**Canonical path**
- `INS/<INSTRUCTOR>/<SERIES>/<CODE>/` (you already use series folders like `PoD/`; keep them)

**Recommended contents**
- `README.md` — index + scope + status
- `VN/` — viewing notes
- `SES/` — training sessions / drill logs
- `TRN/` — raw transcripts (per volume or merged)
- `BIO/` — BIO outputs (full report + partial extracts)
- `ASSETS/` — images/diagrams/screenshots

**Minimum viable**
- `README.md`
- `VN/`
- at least one source artifact folder: `TRN/` or `BIO/` (prefer both)

### 1.3 SYS Folder Standard

**Canonical path**
- `SYS/<system-name>/`

**Recommended contents**
- `README.md` — scope + canonical anti-dup map + source index
- Subfolders are allowed, but keep them stable and minimal.
  - If you already have a working structure (e.g., `positions-ashi/`, `transitions/`, `control-hubs/`, `submissions/`), keep it.

---

## 2. Naming Conventions (Short + Stable)

### 2.1 Instructor Folder
- Stable initials: `GR`, `JD`, `GC`, etc.

### 2.2 Instructional Code Folder
- Short mnemonic code (3–8 chars), stable across repo.

### 2.3 File Naming
- Viewing notes: `VN/VN01.md`, `VN/VN02.md`, …
- Sessions: `SES/S01.md`, `SES/S02.md`, …
- Transcripts: `TRN/V01.md` or `TRN/merged.md` (your choice; be consistent)
- BIO: `BIO/BIO.md` plus optional partials

---

## 3. Index READMEs (Navigation Cost Control)

### 3.1 INS README (Required)
Must contain:
- instructional title + instructor + code
- artifact inventory (TRN present? BIO present? VN coverage)
- quick links to VN, SES, and promoted SYS links (with short “what was promoted” notes)

### 3.2 SYS README (Required)
Must contain:
- scope (in/out)
- canonical map (anti-duplication pointers)
- hub map (positions → transitions → finishes)
- provenance pattern:
  - `Sources: INS/<...>/TRN/... ; INS/<...>/BIO/BIO.md ; INS/<...>/VN/VN0X.md`

---

## 4. End-to-End Workflow (INS → BIO/VN → SYS)

This section defines the canonical sequence for an instructional. The goal is to eliminate repetitive “Next” interactions and make SYS merging a direct follow-on from BIO/VN completion.

### 4.1 Intake (per instructional)
1) Store transcript(s) into `INS/.../TRN/`
2) Ensure `INS/.../README.md` exists and lists volumes + filenames
3) Generate BIO into `INS/.../BIO/BIO.md`
4) Create VN files in `INS/.../VN/` (VN01..VN0N)
5) Record training in `INS/.../SES/` (optional at intake; required once training begins)
6) Merge into `SYS/` using BOA-SYS queue discipline

### 4.2 Batch-first production rule (BIO and VN)
- When generating BIO and VN, use Jigoro Text batch/range/chunk commands to reduce repeated “Next.”
- Default pattern:
  - BIO: `Sections 1-3 (Parts)` first, then `Sections 4-5 (Parts)`, then `Section 6.0 chunked`, then `Sections 7-14 (Parts)`.
  - VN: produce 1–2 volumes per response with explicit stop boundaries (see 5.6).

### 4.3 SYS merge trigger (follow-on from BIO/VN)
Once BIO and VN are complete for an instructional:
- Add the instructional to `META/SOURCE-INDEX.md` (paths to TRN/BIO/VN).
- Start/continue `META/WORK-QUEUE-SYS.md`.
- Merge SYS files using BOA-SYS:
  - one SYS file per response unless explicitly requested otherwise,
  - every SYS update includes “what changed + why,”
  - sources updated to include the new instructional paths.

---

## 5. Viewing Notes Standard (VN)

### 5.1 VN Purpose
- instructional-specific detail at high operational density
- staging layer for SYS extraction (VN is not the canonical system library)

### 5.2 VN Header (Required)
- `# VIEWING NOTES — <Instructional> (<Instructor>)`
- `## VN0X — Volume X`

### 5.3 Standard VN Unit (Per Subchapter)
Use compact unit blocks; omit only if truly absent:
- Objective
- Goal
- Primary decision rule
- Gates
- Controls
- Key concepts
- Primary line
- Positional landmarks
- Mechanics and details
- Coaching cues
- Common errors
- First follow-up (where applicable)
- Branches (defender action → your response)
- Failure-first diagnosis
- Drills (explicit or implied)
- Links (systems / other VN)
- System tags


### 5.4 VN Density Requirement (Operational Grade)
Rules:
- bullets over paragraphs
- no narrative filler
- convert statements into gates/branches whenever possible
- if content is big: split the subchapter

### 5.5 No-invention rule
- VN is allowed to be operator-synthesised, but must not add new technical claims not supported by the instructional artifacts.
- If detail is missing, flag it explicitly.

### 5.6 VN batch delivery protocol (recommended)
When using a batch-capable project/chat:
- Request a bounded batch (prevents overrun):
  - “Output VN01 and VN02 only; stop after VN02.”
- Continue with:
  - “Next x2; stop after VN04.”
- If safe-stop triggers, resume using the Jigoro resume token convention (even though VN is governed by Kano, the transport mechanics apply).

---

## 6. Numbering (Governing Rule)

### 6.1 Volume Mapping
- `VN01` = Volume 1, etc.

### 6.2 Inside-VN Numbering
- use the volume number as major section:
  - `## 5.0 Volume 5`
  - `### 5.1 …`

### 6.3 Timecodes (Optional)
- include only when useful

### 6.4 De-dup / Renumber
- remove duplicates
- renumber to contiguous order
- do not preserve broken numbering for history (Git already does)

---

## 7. Sessions Standard (SES)
Minimum per session:
- focus (1–3 items)
- drills (reps/rounds if possible)
- failures (what broke first)
- fixes (next constraints)
- links to VN/SYS nodes used

---

## 8. Systems Diagrams (When Used)
- diagrams are allowed in SYS and recommended when they reduce ambiguity
- keep ASCII lines ≤130 characters
- use fenced blocks with plain triple-backticks only (no language tag)

---

## 9. Working With Large Transcripts (Non-Negotiable Procedure)

### 9.1 Preferred inputs to minimise failure on huge text
Best → worst:
1) BIO + VN + transcripts available in project files
2) BIO + transcripts
3) VN + transcripts
4) transcripts only

### 9.2 Practical extraction method (how we avoid drowning)
When transcripts are large:
- primary extraction from BIO (structured) + VN (operator synthesis)
- targeted transcript dives only for:
  - confirming phrasing/constraints
  - resolving ambiguity
  - retrieving missing mechanics
  - extracting rules, gates, failure signatures, and if/then branches

### 9.3 Source-of-truth rule
- if VN says X but transcript/BIO implies not-X, SYS must reflect transcript/BIO.
- VN can keep the operator interpretation, but SYS must be evidence-aligned.

### 9.4 Evidence hooks (optional, recommended)
Inside SYS files, optionally add:
- `Evidence hooks:` short bullets tied to BIO/TRN references.

---

## 10. Startup Protocol (Replicate in New Chats With Memory Off)

### 10.1 Required startup packet
When starting a new conversation (or after a reset), paste:

1) Goal statement:
   - “We are updating SYS from multiple instructionals; SYS is canonical; INS is per-instructional.”
2) Working queue:
   - link or paste `META/WORK-QUEUE-SYS.md`
3) Operating agreement:
   - “Follow BOA-SYS (one file at a time unless requested; every update includes what changed + why; queue discipline).”
4) Sources available:
   - confirm what exists as project files (TRN/BIO/VN) for each instructional.

### 10.2 Inputs checklist (fast confirmation)
Before beginning a merge run, confirm:
- Are TRN files present as project files?
- Are BIO outputs present?
- Are VN files present?

Default behavior:
- proceed with BIO/VN as primary; transcripts used by targeted retrieval unless user requests deep mode.

---

## 11. Progress Tracking Artifacts (recommended, repo-level)

Create these in `META/` to prevent queue drift and “where are we?” failures:

1) `META/WORK-QUEUE-SYS.md`
- authoritative ordered list of SYS files
- per-file status: pending | merged | skipped | delta-check
- last updated date + current queue pointer (#n/#N)

2) `META/SOURCE-INDEX.md`
- instructionals in scope → their INS paths
- what artifacts exist for each (TRN/BIO/VN)

3) `META/CHANGELOG-SYS-MERGES.md` (optional)
- short per-run log: date, instructionals included, files updated, notable deltas

---

## 12. Operating Rules (Do Not Break)

- SYS is canonical and merged. INS is detailed and per-instructional.
- Default: one file at a time output (unless explicitly requested).
- For every SYS update, include:
  - what changed
  - why it changed
- No silent queue switching:
  - queue is governed by `META/WORK-QUEUE-SYS.md` unless you explicitly override.

---
