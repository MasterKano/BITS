PATH: BOA-SYS.md

# BITS Ops Agreement — SYS Merge Workflow (BOA-SYS) v0.6

## 0. Purpose (binding)
This agreement defines the binding operational workflow for merging instructionals into the canonical `SYS/` systems database.

It exists to prevent:
- duplicate SYS pages,
- low-signal summary content,
- uncontrolled drift from the merge queue,
- silent changes without justification,
- SYS pages that omit defence logic where defence exists in source instructionals,
- SYS merges that proceed without first producing VN and BIO from transcripts.

### 0.1 Primary operating assumption
- You upload **transcripts (TRN) only**.
- VN and BIO are produced from TRN inside the project workflow, then promoted into SYS.

### 0.2 Pipeline (canonical)
**TRN → VN → BIO → SYS**

This agreement governs the **SYS phase** and the controls required to keep SYS canonical, deduplicated, and operator-grade.

### 0.3 Draft vs Published (operating definitions)
- **Draft:** content not yet pasted into GitHub; may change rapidly.
- **Published:** content pasted into GitHub; treated as binding until the next version bump.

---

## 1. Scope and Boundaries

### 1.1 What this agreement governs
- SYS merge queue execution (file-by-file)
- Instructional → SYS handoff rules
- Source intake rules (Project files vs pasted text)
- Output contract (copy/paste safe)
- Change reporting requirements (“what changed and why” every time)
- Diagram rules (ASCII, width discipline)
- Defence integration rule (attack + defence combined in SYS by default)
- Batch-safe execution for SYS merges

### 1.2 What this agreement does *not* govern
- BIO report creation rules and formatting (Jigoro Text governs)
- VN or session standards (Kano Scroll governs)
- Repo restructuring unless explicitly requested

---

## 2. Canonical Principle (non-negotiable)
- `SYS/` is the **single merged system library**.
- If a topic already exists in `SYS/`, we **update that file** rather than creating a duplicate.
- `INS/` holds instructional-specific artifacts (TRN/VN/BIO).
- `SYS/` holds the durable, merged, instructional-agnostic system view.

---

## 3. Instructional Lifecycle Gate (binding)

### 3.1 Mandatory lifecycle order
SYS merge may not begin for an instructional until the following are complete:

1. **TRN intake** (source-of-truth)
2. **VN generated** (Titles-aligned when Titles file exists)
3. **BIO generated** (template-locked per Jigoro Text)
4. **SYS merge** (this agreement)
5. **Delta check**
6. **Queue advancement**

Skipping steps 2 or 3 is not permitted unless you explicitly instruct otherwise.

### 3.2 SYS merge entry criteria (gate)
Before SYS merge starts, the following must exist in project files or be pasted in chat:
- BIO file (`INS/.../BIO/BIO.md` or equivalent)
- VN files (`INS/.../VN/VN01..VN0N`, or declared partial scope)

If only TRN exists, the correct action is to generate VN and BIO first (Kano/Jigoro), then begin SYS.

---

## 4. Inputs and Source Hierarchy

### 4.1 Preferred delivery method: Project files
Default preference: all sources live in project files for persistence and explicit provenance.

### 4.2 Source hierarchy (binding)
- **VN + BIO** = primary SYS merge inputs (operator-grade structure + condensed logic)
- **TRN** = source-of-truth and audit layer (used to resolve ambiguity/conflict)

### 4.3 Source-of-truth rule (binding)
If VN/BIO conflicts with TRN, SYS must follow TRN.

### 4.4 When transcripts are used
TRN is used:
- when VN/BIO are thin, ambiguous, or internally inconsistent,
- when explicitly requested,
- when building a first-time canonical hub/system page,
- during delta checks.

### 4.5 Transcript retrieval modes (declared)
For any SYS update using TRN, one mode must be stated in the delta summary:
- **Targeted (default):** keyword + concept pulls only
- **Deep:** system-first sweep (explicitly requested or required for first-time canonical build)
- **Delta:** contradiction/gap audit after merge

### 4.6 Provenance floor (non-negotiable)
Any non-obvious new technical content must be grounded in at least one of:
- BIO reference, and/or
- TRN reference (if TRN used)

VN is an operator synthesis layer; VN-only claims are not canonical unless explicitly marked provisional by user instruction.

---

## 5. Queue Discipline

### 5.1 Single queue rule
- One active SYS queue.
- Executed top-to-bottom.
- No jumping unless explicitly instructed.

### 5.2 Queue artifact (binding)
The queue must exist in the repo as:
`META/WORK-QUEUE-SYS.md`

This file is authoritative for:
- file order,
- status (`pending | merged | skipped | delta-check`),
- resume notes.

If chat state conflicts with repo queue, repo queue wins unless overridden.

### 5.3 “What’s next?” protocol
When asked “What’s next?”, return:
- next SYS file path,
- merge type (update vs create),
- required sources (BIO/VN/TRN),
- queue position (`#n / #N`).

### 5.4 Per-update status (required)
Every SYS response must state:
- queue position,
- file status,
- skip reason (if skipped),
- next file.

---

## 6. Output Contract

### 6.1 One-file-per-response (default)
Default: exactly one SYS file per response.
Multiple files only when explicitly requested.

### 6.2 File header (locked)
First line must be:
`PATH: <relative/path>.md`

### 6.3 Copy/paste safety (locked)
- Deliverable returned in one fenced markdown block.
- No extra content inside the block.

### 6.4 Density standard (locked)
Operator-grade only:
- decision rules,
- gates,
- failure signatures,
- transition logic,
- defence triggers → attacker responses.

No narrative filler.

---

## 7. Change Reporting (mandatory)

Every SYS update must include outside the code block:

### 7.1 Delta Summary (required fields)
- **Added**
- **Modified**
- **Removed** (only if necessary)
- **Why**
- **Sources touched** (INS paths added/used)

### 7.2 No silent deviations
Any deviation from:
- queue order,
- structure/numbering,
- diagram rules,
must be explicitly declared and justified.

### 7.3 Conflicting instructionals
If instructionals disagree:
- preserve both as named variants,
- add a selection rule,
- never silently delete.

---

## 8. Systems Page Standard

### 8.1 Section numbering (locked)
SYS pages use numbered sections (e.g., `## 1. Purpose`).
Legacy structures are preserved unless migration is requested.

### 8.2 Combined attack + defence rule (binding)
Default: SYS pages combine attack and defence by default.
Enforced by:
1. inserting a Defence Model section if missing,
2. integrating defence as defender triggers → attacker responses,
3. creating defence-only pages only when content is cross-hub reusable and clearly separable.

### 8.3 SYS extraction gate (binding)
Before writing/updating any SYS node from an instructional:
- VN Titles-alignment lint has passed (Kano governs this),
- lumped transcript remediation completed where applicable (Kano governs this),
- system is expressed in SYS form:
  - gates, decision rules, failure patterns, minimal technique anchors.

---

## 9. ASCII Diagram Standard

### 9.1 Requirement
At least one diagram per SYS page when it improves clarity.

### 9.2 Constraints (locked)
- ≤120 characters per line
- Plain triple-backtick fence only
- No language tags

### 9.3 Conventions (recommended)
- `[HUB]` = platform
- `(OUTCOME)` = finish / sweep / top
- `{OR}` = branch
- `!` = gate / failure

### 9.4 Broken diagram remediation
If a diagram renders incorrectly:
- next response reissues diagram only,
- include one-line fix note.

---

## 10. Delta Check Loop
After queue completion:
- verify instructional coverage,
- verify density,
- verify diagrams,
- verify links and canonical map,
- verify attack + defence integration,
- run a contradiction scan (new vs existing SYS claims).

---

## 11. Decision Surfacing
Whenever a decision is required, state:
- decision,
- why it matters,
- default recommendation,
- alternatives.

Blockers must include:
- what is blocked,
- minimal unblock input,
- what can proceed next.

---

## 12. Versioning and Changelog (locked)
Every published change requires a version bump.

### 12.1 Changelog
- **v0.6 (from v0.5)**
  - Reframed workflow for TRN-only uploads: TRN → VN → BIO → SYS.
  - Clarified SYS merge gate: SYS begins only after VN + BIO exist (derived from TRN).
  - Explicitly stated TRN as source-of-truth with VN/BIO as primary merge inputs.
  - Aligned diagram width rule to ≤120 chars/line and removed ambiguity.
  - Added SYS extraction gate tying SYS readiness to Kano lint/remediation.
  - Expanded delta summary to require “Sources touched.”

End — BOA-SYS v0.6
