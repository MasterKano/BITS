PATH: Kano-Scroll.md

# Kano Scroll v4.2 — BITS Training Guidance Manual (PUBLISHED)

## 0. Purpose

This manual governs how to convert **transcripts (TRN)** into:
- **VN** (Viewing Notes): high-density operator notes, Titles-aligned
- **BIO**: structured report (template-locked per Jigoro Text)
- **SYS**: your evolving systems database (canonical, deduped library)

### 0.1 Primary operating assumption
- **You only upload transcripts.**
- Everything else (VN, BIO, SYS updates) is derived from TRN.

### 0.2 Pipeline (canonical)
**TRN → VN → BIO → SYS**

### 0.3 Scope boundaries
- **Kano Scroll** = repo structure, naming/numbering, VN standards, SYS promotion workflow, diagram constraints, correction protocol.
- **Jigoro Text** = BIO generation rules, BIO template, and delivery grammar.
- **BOA-SYS** = SYS merge operating agreement (queue discipline + delta reporting). Applies in SYS phase only.

---

## 1. Repository Layout (Canonical)

### 1.1 Root
- `INS/` — instructionals workspace (TRN + VN + BIO + assets)
- `SYS/` — systems database (canonical, deduped)
- `TEMPLATES/` — templates (VN skeleton, BIO skeleton, SYS node skeleton)
- `META/` — indexes and queues (recommended, light-weight)

### 1.2 INS Folder Standard
**Canonical path**
- `INS/<INSTRUCTOR>/<SERIES>/<CODE>/`

**Required contents**
- `README.md` — inventory + status + pointers
- `TRN/` — transcripts (source-of-truth)
- `VN/` — viewing notes (derived)
- `BIO/` — BIO report outputs (derived)

**Recommended**
- `ASSETS/` — diagrams, screenshots
- `SES/` — training session logs (optional but useful)

### 1.3 SYS Folder Standard
**Canonical path**
- `SYS/<system-name>/`

**Required**
- `README.md` — scope, canonical anti-dup map, sources index
- system nodes (files) as required by your taxonomy

---

## 2. Naming Conventions (Canonical)

### 2.1 Instructional Code
- Use a stable code per instructional, e.g. `NWJJ-OG-P1`
- Put the code in:
  - INS folder name
  - INS README header
  - BIO report header
  - Transcript filenames

### 2.2 Transcript Filenames (TRN)
- `TRN_<CODE>_Vol_01.docx`
- `TRN_<CODE>_Vol_02.docx`
- …

### 2.3 VN Filenames
- `VN01.md`, `VN02.md`, …, `VN0N.md`

### 2.4 BIO Filename
- `BIO.md` (single canonical report file per instructional)

### 2.5 Session Filenames (optional)
- `SES_YYYY-MM-DD.md`

---

## 3. Index READMEs (Navigation Cost Control)

### 3.1 INS README (Required)
Must contain:
- instructional title + instructor + code
- TRN inventory (volumes + filenames)
- VN coverage status (VN01..VN0N present?)
- BIO status (BIO present? sections complete?)
- SYS promotion log (what was extracted/updated in SYS)

### 3.2 SYS README (Required)
Must contain:
- scope (in/out)
- canonical anti-dup map (where the “true” definition lives)
- hub map (positions → transitions → finishes)
- provenance (minimum):
  - `Sources: INS/<...>/TRN/... ; INS/<...>/BIO/BIO.md ; INS/<...>/VN/VN0X.md`

---

## 4. End-to-End Workflow (TRN → VN → BIO → SYS)

### 4.1 Intake (per instructional)
1) Store transcripts into `INS/.../TRN/`
2) Create/update `INS/.../README.md` with volume list + filenames
3) Generate VN volumes into `INS/.../VN/` (Titles-aligned)
4) Generate BIO into `INS/.../BIO/BIO.md` (Jigoro template)
5) Extract/update SYS nodes from VN/BIO (BOA-SYS discipline)

### 4.2 Production rule (batch-first)
- Default production order:
  - VN first (structure + mechanics capture)
  - BIO second (report consolidation)
  - SYS last (dedupe + canonicalization)

### 4.3 Source-of-truth rule (hard)
- **TRN is authoritative.**
- VN and BIO are derived; if conflict exists, SYS must follow TRN.

---

## 5. Viewing Notes Standard (VN)

### 5.1 VN purpose
- Capture instructional content at operational density.
- Provide clean structure for BIO and SYS extraction.

### 5.2 VN header (required)
- `# VIEWING NOTES — <Instructional> (<Instructor>)`
- `## VN0X — Volume X`

### 5.3 Titles file outline authority (mandatory when provided)
If a Titles file (chapter/subchapter list) exists:
- Titles is the controlling outline for:
  - VN subchapter headings and ordering
  - inside-VN numbering (`X.1 … X.n`)
  - diagram chapter labeling
- Transcript-driven segmentation is subordinate:
  - if transcript text is merged/lumped, it must be re-parsed to match Titles subchapters
  - do not invent subchapters or rename Titles headings for convenience
- If a Titles subchapter appears missing, assume it is embedded until proven absent (see 9.5).

### 5.4 Standard VN unit (per subchapter)
Minimum fields (do not omit):
- Objective
- Primary decision rule
- Gates/constraints
- Common errors / failure signatures

Recommended fields (use when supported by TRN):
- Controls / handles
- Key concepts
- Positional landmarks
- Mechanics and details
- Coaching cues
- Branches (opponent action → your response)
- Failure-first diagnosis
- Drills (explicit or implied)
- Links (to other subchapters / SYS nodes)
- System tags

### 5.5 VN density requirement (operational grade)
Rules:
- bullets over paragraphs
- minimize narrative filler
- convert statements into gates/branches whenever possible
- if a subchapter is large: split internally with short labeled blocks (do not change Titles headings)

### 5.6 No-invention rule
- VN is allowed to synthesize, but must not add technical claims not supported by TRN.
- If detail is absent, flag it explicitly.

### 5.7 VN delivery protocol (recommended)
- Produce bounded sets:
  - “VN01 only; stop.”
  - “Next x2; stop after VN03.”
- Corrections must use Patch Protocol (see 5.9).

### 5.8 Titles-alignment lint step (mandatory pre-output check)
Before delivering any VN volume (or reissuing):
- All Titles subchapters present and in order (`X.1 … X.n`)
- Headings match Titles wording (minor punctuation normalization only)
- No subchapter is silently merged
- Minimum VN unit fields present (Objective + Decision rule + Gates + Errors)
- If any fail: fix structure first, then refine density

### 5.9 Patch protocol for corrections (low-noise reissues)
When correcting an already-delivered VN:
- Reissue only the affected range (e.g., “VN6 §6.4–6.5”)
- Include a short delta header (max 4 lines):
  - Changed:
  - Moved:
  - Added:
  - Unresolved:
- Maintain existing density unless explicitly instructed otherwise

---

## 6. Numbering (Governing Rule)

### 6.1 Volume mapping
- `VN01` = Volume 1, etc.

### 6.2 Inside-VN numbering
- `## X.0 Volume X`
- `### X.1 …`

### 6.3 Timecodes and timestamp conflict policy
- Timecodes are optional; include only when they reduce ambiguity.
- Precedence:
  1) TRN timecodes (highest)
  2) Titles time ranges
  3) none
- If Titles time ranges are inconsistent/non-linear:
  - keep them as labels only
  - preserve Titles order (do not reorder content to “fit”)

---

## 7. Sessions Standard (SES) (Optional)
Minimum per session:
- focus (1–3 items)
- drills (reps/rounds if possible)
- failures (what broke first)
- fixes (next constraints)
- links to VN and SYS nodes used

---

## 8. Systems Diagrams (When Used)
- Diagrams are allowed and recommended when they reduce ambiguity.
- Constraints:
  - ASCII only
  - width ≤120 characters per line (hard-wrap if needed)
  - fenced blocks: plain triple-backticks only (no language tags)
- Diagrams should express:
  - gates, branches, and failure points (not just a table of contents)

---

## 9. Working With Transcripts (Non-Negotiable Procedure)

### 9.1 Inputs (operating assumption)
- TRN is the only required input.
- Titles file is optional but becomes mandatory authority if provided.

### 9.2 Practical extraction method
- Primary extraction produces VN (Titles-aligned).
- BIO is built from VN + TRN confirmation where needed (Jigoro governs).
- Targeted TRN dives are required when:
  - resolving ambiguity
  - confirming constraints/gates
  - recovering missing mechanics
  - repairing lumped/merged transcript sections

### 9.3 Evidence rule for SYS promotion
- SYS claims must be traceable to TRN:
  - directly (quoted/confirmed mechanics), or
  - indirectly via VN/BIO that is explicitly TRN-derived

### 9.4 SYS extraction gate (mandatory before SYS updates)
Before updating/adding any SYS node from an instructional:
- VN Titles-alignment lint passed (5.8)
- Lumped transcript remediation completed if needed (9.5)
- System is expressed in canonical SYS form:
  - gates
  - decision rules
  - failure patterns
  - minimal technique anchors (only as needed to implement the system)

### 9.5 Lumped transcript remediation (required)
When TRN merges multiple subchapters into a single block:
- Assume missing material is embedded nearby.
- Re-parse by signals in this order:
  1) stated purpose
  2) opponent reaction / defense
  3) corrective rule / constraint
  4) hub/position change
- Extract and relocate into the correct Titles subchapter(s).
- Only after targeted scan may you declare “missing content,” and you must state:
  - which subchapter is missing
  - what evidence was checked (TRN range)

---

## 10. SYS Phase (Downstream; BOA-SYS Applies Here)

### 10.1 What SYS is
- SYS is the canonical, deduplicated systems database.
- INS contains instructional-specific artifacts (TRN/VN/BIO).

### 10.2 When BOA-SYS applies
- BOA-SYS rules apply **only** during SYS updates/merges.
- VN/BIO generation is governed by Kano/Jigoro; SYS merging is governed by BOA-SYS.

### 10.3 SYS update discipline (summary)
- One SYS file/node per change-set unless explicitly requested otherwise.
- Every update includes a delta:
  - what changed
  - why it changed
  - which sources were added (INS paths)

---

## 11. Startup Protocol (New Chats / Resets)

### 11.1 Required startup packet
Paste:
1) Instructional code + instructor + series
2) TRN inventory (volumes + filenames)
3) Titles file status (present? authoritative)
4) Current work target:
   - VN volume(s) range, or
   - BIO section(s) range, or
   - SYS node to update

---

## 12. Hard Rules (Do Not Violate)

- TRN is the only required input and the source-of-truth.
- If a Titles file is provided, it controls subchapter structure and naming.
- Do not rotate/spin under stable base when the system requires a base-break gate.
- Keep ASCII diagrams ≤120 chars/line and in plain triple-backtick fences only.
- Corrections must use Patch Protocol and must not silently merge subchapters.
