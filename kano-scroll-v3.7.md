# Kano Scroll v3.8 — BITS Training Guidance Manual (PUBLISHED)

## 0. Purpose

- Provide a repeatable method to learn and train from grappling instructionals using:
  - `INS/` — per-instructional workspace (VN + sessions + source artifacts)
  - `SYS/` — one unified, deduplicated systems library
- Enforce provenance for anything promoted into `SYS/`:
  - [I] raw transcript (source-of-truth) and/or
  - [B] BIO report generated from transcript
  - VN is allowed as an intermediate “operator note layer,” but SYS claims must remain traceable to I/B.
- Separate manuals, separate scopes:
  - **Kano Scroll** = repo structure, naming/numbering, VN/session standards, SYS promotion workflow, startup protocol.
  - **Jigoro Text** = BIO generation rules and formatting.

---

## 1. Repository Layout (Canonical)

### 1.1 Root

- `INS/` — Instructionals (one folder per instructional)
- `SYS/` — Systems library (canonical, merged, deduped)
- `TEMPLATES/` — copy/paste templates (VN, sessions, SYS skeletons)
- `META/` — indexes + conventions + operational notes (recommended)

### 1.2 INS Folder Standard

**Canonical path**
- `INS/<INSTRUCTOR>/<CODE>/`

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
  - If starting fresh, prefer one of:
    - **Option A (simple):** `positions/`, `transitions/`, `submissions/`, `control/`
    - **Option B (current leglocks style):** `positions-ashi/`, `transitions/`, `control-hubs/`, `submissions/`

---

## 2. Naming Conventions (Short + Stable)

### 2.1 Instructor Folder

- Stable initials: `GR`, `JD`, `GC`, etc.

### 2.2 Instructional Code Folder

- Short mnemonic code (3–8 chars), stable across repo.
- Example: `INS/GR/SAL/` = Systematically Attacking the Legs

### 2.3 File Naming

- Viewing notes: `VN/VN01.md`, `VN/VN02.md`, …
- Sessions: `SES/S01.md`, `SES/S02.md`, …
- Transcripts: `TRN/V01.md` or `TRN/merged.md` (your choice; be consistent)
- BIO: `BIO/BIO.md` plus optional partials (`BIO/technique-library.md`, etc.)

---

## 3. Index READMEs (Navigation Cost Control)

### 3.1 INS README (Required)

Must contain:
- instructional title + instructor + code
- artifact inventory:
  - transcripts present? (TRN)
  - BIO present? (BIO)
  - VN coverage (VN01..VNxx)
- quick links:
  - VN list
  - SES list
  - any promoted SYS links (with short notes: “what was promoted”)

### 3.2 SYS README (Required)

Must contain:
- scope (in/out)
- canonical map (anti-duplication pointers)
- hub map (positions → transitions → finishes)
- provenance pattern:
  - `Sources: INS/<INSTRUCTOR>/<CODE>/TRN/... ; INS/<INSTRUCTOR>/<CODE>/BIO/... ; INS/<INSTRUCTOR>/<CODE>/VN/VN0X.md`

---

## 4. Workflow (INS → SYS Promotion)

### 4.1 Intake (per instructional)

1) Store transcript(s) into `INS/.../TRN/`
2) Generate BIO into `INS/.../BIO/`
3) Create/extend VN in `INS/.../VN/`
4) Record training in `INS/.../SES/`

### 4.2 Promotion Rule (SYS is curated)

Promote only when a concept is reusable and can be expressed as:
- **conditions → actions → constraints → branches → outcomes**

Promotion method:
- update the existing canonical SYS node if it exists (no duplicates)
- add/extend:
  - gates
  - decision rules
  - failure signatures
  - transitions/outcomes
  - drills

### 4.3 SYS Merge Loop (Operational)

For each SYS file being updated:

1) **Baseline**
   - start from current SYS file (existing canonical)
2) **Ingest**
   - pull candidate deltas from BIO/VN
   - use transcript only to confirm/clarify/expand (see §9)
3) **Merge**
   - integrate deltas without changing your header structure unless necessary
4) **Delta note (mandatory)**
   - append or provide alongside: “What changed / why”
5) **Source hygiene**
   - update `Sources` list with the specific INS paths used

---

## 5. Viewing Notes Standard (VN)

### 5.1 VN Purpose

- instructional-specific detail at high operational density
- staging layer for SYS extraction (VN is not the canonical system library)

### 5.2 VN Header (Required)

At top of each VN:
- `# VIEWING NOTES — <Instructional> (<Instructor>)`
- `## VN0X — Volume X`

### 5.3 Standard VN Unit (Per Subchapter)

Use compact unit blocks; omit only if truly absent:
- key concepts
- position/structure
- decision rules (if/then)
- cues/checkpoints
- failure modes
- drills (explicit or implied)
- system tags

### 5.4 VN Density Requirement (Operational Grade)

Rules:
- bullets over paragraphs
- no narrative filler
- convert statements into gates/branches whenever possible
- if content is big: split the subchapter

Minimum operational payload (when applicable):
- objective (1 line)
- gates (2–6 bullets)
- controls (2–8 bullets)
- primary line (3–10 bullets)
- branches (≥2)
- failure-first diagnosis (1–5 bullets)

---

## 6. Numbering (Governing Rule)

### 6.1 Volume Mapping

- `VN01` = Volume 1, etc.

### 6.2 Inside-VN Numbering

- use the volume number as major section:
  - `## 5.0 Volume 5`
  - `### 5.1 …`

### 6.3 Timecodes (Optional)

- include only when useful:
  - `### 5.7 Countering X (12:34)`

### 6.4 De-dup / Renumber

- remove duplicates
- renumber to contiguous order
- do not preserve broken numbering “for history” (Git already does)

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

- diagrams are allowed in `SYS/` and recommended when they reduce ambiguity
- keep ASCII lines ≤130 characters
- use fenced blocks with plain triple-backticks (no language tag)

---

## 9. Working With Large Transcripts (Non-Negotiable Procedure)

### 9.1 Preferred input to minimise failure on huge text

Best → worst:
1) **BIO + VN + transcripts available in project files**
2) BIO + transcripts
3) VN + transcripts
4) transcripts only (slowest, highest risk of missing details)

### 9.2 Practical extraction method (how we avoid “drowning”)

When transcripts are large:
- **Primary extraction** from BIO (structured) + VN (operator synthesis)
- **Targeted transcript dives** only for:
  - confirming phrasing/constraints
  - resolving ambiguity
  - retrieving missing mechanics
  - extracting “rules,” “gates,” “failure signatures,” and “if/then” branches

### 9.3 Source-of-truth rule

- if VN says X but transcript/BIO implies not-X, SYS must reflect transcript/BIO.
- VN can keep the “operator interpretation,” but SYS must be evidence-aligned.

### 9.4 “Evidence hooks” (recommended)

When you want tighter traceability, add inside SYS files:
- `Evidence hooks:` short bullets like:
  - `- ETS LL: toe hold used to force unlock/separation (BIO ref + TRN ref)`
(You can keep this minimal; it’s optional.)

---

## 10. Startup Protocol (Replicate in New Chats With Memory Off)

Use this when you start a new conversation or reset:

1) State goal:
   - “We are updating SYS from multiple instructionals; SYS is canonical; INS is per-instructional.”
2) State working queue:
   - list the exact file paths in the intended order
3) State workflow:
   - “You give merged file content one file at a time; for each update you must include: what changed + why.”
4) Provide sources available:
   - “Project files include: TRN/BIO/VN for X instructionals.”
5) Run:
   - user pastes current SYS file → assistant returns merged SYS file + delta notes → next file.

---

## 11. Operating Rules (Do Not Break)

- SYS is canonical and merged. INS is detailed and per-instructional.
- One file at a time output.
- For every SYS update, include:
  - **What changed**
  - **Why it changed**
- No silent queue switching: if the queue changes, state the change and the reason before continuing.

---
