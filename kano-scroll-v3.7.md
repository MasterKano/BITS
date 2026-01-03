# Kano Scroll v3.7 — BITS Training Guidance Manual

## 0. Purpose

- Provide a repeatable method to learn and train from grappling instructionals using:
  - `INS/` (per-instructional workspace: VN + sessions + transcript/BIO storage)
  - `SYS/` (one unified system library; deduplicated; promotion-based)
- Enforce provenance:
  - Content promoted to `SYS/` must be derived from:
    - [I] raw transcript (source-of-truth)
    - [B] BIO report generated from transcript (structured extraction)
- Separate manuals, separate scopes:
  - **Kano Scroll** governs: repo structure, naming/numbering, VN/session standards, SYS promotion workflow.
  - **Jigoro Text (BIO Instructions)** governs: BIO generation rules and formatting.

---

## 1. Repository Layout (Canonical)

### 1.1 Root

- `INS/` — Instructionals (one folder per instructional)
- `SYS/` — Systems library (deduplicated technical library)
- `TEMPLATES/` — Copy/paste templates (VN, sessions, SYS skeletons)
- `META/` — Indexes + conventions + tooling notes (optional but recommended)

### 1.2 INS Folder Standard

**Canonical path:**
- `INS/<INSTRUCTOR>/<CODE>/`

**Inside (recommended):**
- `README.md` (index: quick links, status, scope)
- `VN/` (viewing notes)
- `SES/` (training sessions / drill logs)
- `TRN/` (raw transcripts; per volume or merged)
- `BIO/` (BIO output files; full report + partials)
- `ASSETS/` (images/screenshots/diagrams if needed)

**Minimum viable:**
- `README.md`
- `VN/`
- At least one source artifact folder: `TRN/` or `BIO/`

### 1.3 SYS Folder Standard

**Canonical path:**
- `SYS/<system-name>/`

**Inside (recommended):**
- `README.md` (overview + canonical anti-dup map)
- `MAP.md` (one-screen map: hubs → transitions → finishes)
- `POS/` (positions / entanglements / hubs)
- `TRN/` (transitions)
- `SUB/` (submissions / finishing mechanics)
- `DEF/` (defence / escapes / counter-logic)
- `DRL/` (drills / progressions)
- `REF/` (terminology + assumptions + constraints)

---

## 2. Naming Conventions (Short + Stable)

### 2.1 Instructor Folder

- Use stable initials: `GR`, `JD`, `GC`, etc.

### 2.2 Instructional Code Folder

- Use short mnemonic code (3–8 chars), stable across repo.
- Example:
  - `INS/GR/SAL/` = Systematically Attacking the Legs

### 2.3 File Naming (Low Friction)

- Viewing notes:
  - `VN/VN01.md`, `VN/VN02.md`, …
- Sessions:
  - `SES/S01.md`, `SES/S02.md`, … (chronological)

---

## 3. Index READMEs (Reduce Navigation Cost)

### 3.1 INS README (Required)

Must contain:
- Instructional title + instructor + code
- Artifact inventory:
  - transcripts present? (TRN)
  - BIO present? (BIO)
  - VN coverage (VN01..VNxx)
- Quick links:
  - VN files list
  - session files list
  - any promoted SYS links

### 3.2 SYS README (Required)

Must contain:
- Scope statement (in/out)
- Canonical map (anti-duplication pointers to other SYS nodes)
- Hub map (positions → transitions → finishes)
- Provenance:
  - `Sources: INS/<INSTRUCTOR>/<CODE> (TRN + BIO + VN refs)`

---

## 4. Workflow (INS → SYS Promotion)

### 4.1 Intake

1) Store transcript(s) into `INS/.../TRN/`
2) Generate BIO report into `INS/.../BIO/`
3) Create `INS/.../VN/` while watching
4) Record training into `INS/.../SES/`

### 4.2 Promotion Rule (SYS is curated)

Promote only when a concept is reusable and can be expressed as:
- conditions → actions → constraints → branches → outcomes

Promotion method:
- Create/extend SYS nodes (`POS/`, `TRN/`, `SUB/`, `DEF/`, `DRL/`)
- Add provenance line(s) inside the SYS file:
  - `Sources: INS/<INSTRUCTOR>/<CODE>/TRN/... ; INS/<INSTRUCTOR>/<CODE>/BIO/... ; INS/<INSTRUCTOR>/<CODE>/VN/VN0X.md`

---

## 5. Viewing Notes Standard (VN)

### 5.1 VN Purpose

- Capture instructional-specific detail at high density.
- Encode decision rules and mechanics in a promotion-ready shape.
- Serve as the staging area for SYS extraction (not the final library).

### 5.2 VN File Header (Required)

At top of each VN:
- Title
- Volume
- Optional tag line

Recommended:
- `# VIEWING NOTES — <Instructional> (<Instructor>)`
- `## VN0X — Volume X`

### 5.3 Standard VN Unit (Per Subchapter)

Each subchapter should use the same compact “unit” blocks (omit blocks only if truly absent):

- Key concepts
- Position–structure
- Decision rules (if/then)
- Key cues (checkpoints + tells)
- Failure modes (what breaks first)
- Drills (if provided or obviously implied by the material)
- System tags (single line)

### 5.4 VN Density Requirement — High Operational Grade (Mandatory)

Viewing Notes must be written to “operational grade density,” meaning:
- No narrative filler.
- Preference for actionable constraints and branch logic over description.
- Every meaningful concept is expressed as a *repeatable decision or mechanic*.

Minimum “operational” content per subchapter (when applicable):
- **Objective:** what you are trying to accomplish (one line)
- **Gates:** what must be true before progressing (2–6 bullets)
- **Controls:** what holds the position together (2–8 bullets)
- **Primary line:** preferred attack/transition line (3–10 bullets)
- **Branches:** defender action → your response (at least 2 if present)
- **Failure-first diagnosis:** what to fix first when it fails (1–5 bullets)

Formatting rules to keep speed high:
- Use bullets, not paragraphs.
- Prefer compact nouns/verbs (“knee-line trapped”, “hands high”, “hip wedge”).
- If a topic is big, split into two subchapters rather than bloating one.
- If something repeats across volumes (e.g., “hands high”), keep it as a short cue and rely on tags rather than re-explaining.

---

## 6. 1C — Standardise Numbering (Governing Rule)

### 6.1 Volume Mapping

- `VN01` = Volume 1
- `VN02` = Volume 2
- etc.

### 6.2 Numbering Inside a VN

- Use the volume number as the major section.
  - Example (Volume 5):
    - `## 5.0 Volume 5`
    - `### 5.1 …`
    - `### 5.2 …`

### 6.3 Timecodes (Optional, Recommended)

- Include timecodes in the heading only when available and useful:
  - `### 5.7 Countering X (12:34)`

### 6.4 De-duplication / Renumbering Rule

- If duplication exists (copy/paste repeats), remove duplicates.
- If numbering is broken, renumber to restore contiguous order.
- Do not preserve old numbering “for history” inside VN files; Git already tracks history.

---

## 7. Sessions Standard (SES)

- Purpose: record what you drilled, what failed, and what changes next session.
- Minimal per session:
  - Focus (1–3 items)
  - Drills (exact reps/rounds if possible)
  - Failures (what broke first)
  - Fixes (next constraints)
  - Links to VN/SYS nodes relevant to the session

---

## 8. System Tags Standard

- Use tags to reduce repetition and improve searchability.
- Format:
  - `- System tags: tag-a, tag-b, tag-c`
- Prefer stable tags; avoid synonyms unless needed.
  - Example: choose one of `knee-line` vs `knee-line-control` (not both).

---