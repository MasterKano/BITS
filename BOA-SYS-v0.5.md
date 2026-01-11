PATH: BOA-SYS.md

# BITS Ops Agreement — SYS Merge Workflow (BOA-SYS) v0.5

## 0. Purpose (binding)
This agreement defines the **binding operational workflow** for merging multiple instructionals into **canonical SYS pages** in BITS.

It exists to prevent:
- duplicate system pages,
- low-signal “summary” content,
- uncontrolled drift from the agreed queue,
- silent changes without a reason given,
- SYS pages that omit defence logic when defence instructionals are merged,
- and SYS merges that proceed without first consuming the instructional’s BIO and VN.

This agreement governs **how SYS work is executed**.  
It does **not** replace Kano Scroll (repo / training manual) nor Jigoro Text (BIO standard).

### 0.1 Draft vs Published (operating definitions)
- **Draft:** content not yet pasted into GitHub; may change rapidly.
- **Published:** content pasted into GitHub; treated as binding until the next version bump.

---

## 1. Scope and Boundaries

### 1.1 What this agreement governs
- SYS merge queue execution (file-by-file)
- Instructional → SYS handoff rules
- Source intake rules (Project files vs pasted text)
- Output format rules (copy/paste safe)
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
- `INS/` holds per-instructional detail (BIO / VN / transcripts).
- `SYS/` holds the **durable, merged, instructional-agnostic system view**.

---

## 3. Instructional Lifecycle Gate (binding)

### 3.1 Mandatory lifecycle order
SYS merge **may not begin** for an instructional until the following are complete:

1. **TRN intake** (once per instructional)
2. **BIO generated** from transcript(s)
3. **VN generated** from BIO + transcript(s)
4. **SYS merge** (this agreement)
5. **Delta check**
6. **Queue advancement**

Skipping steps 2 or 3 is **not permitted** unless you explicitly instruct otherwise.

### 3.2 SYS merge entry criteria (gate)
Before SYS merge starts, the following **must exist in project files or be pasted in chat**:
- BIO file (`INS/.../BIO/BIO.md` or equivalent)
- VN files (`VN01..VN0N`, or declared partial scope)

If BIO/VN were created in another project, they **must be uploaded** before SYS work proceeds.

---

## 4. Inputs and Source Hierarchy

### 4.1 Preferred delivery method: Project files
Default preference: all sources live in **project files**.

Why:
- persistence across turns,
- explicit provenance,
- clean cross-chat replication.

### 4.2 Source hierarchy (binding)
- **BIO + VN** = primary SYS merge inputs
- **Transcripts (TRN)** = audit layer only

### 4.3 When transcripts are used
TRN is used:
- when BIO/VN are thin or inconsistent,
- when explicitly requested,
- when building a first-time canonical hub,
- during delta checks.

### 4.4 Transcript retrieval modes
Large transcripts are handled using one declared mode:

- **Targeted (default):** keyword + concept pulls only
- **Deep:** system-first sweep (explicitly requested)
- **Delta:** contradiction / gap audit after merge

For any SYS update using TRN, the delta summary must state:
- mode used,
- keywords / chapters scanned,
- what was added because of TRN.

Line-by-line transcript rewrites are **never** default behavior.

### 4.5 Provenance floor (non-negotiable)
Any **non-obvious new technical content** must be grounded in at least one of:
- BIO reference, and/or
- TRN reference (if TRN used).

VN is an operator synthesis layer; VN-only claims are **not canonical** unless explicitly marked provisional by user instruction.

---

## 5. Queue Discipline

### 5.1 Single queue rule
- One active SYS queue.
- Executed top-to-bottom.
- No jumping unless explicitly instructed.

### 5.2 Queue artifact (binding)
The queue **must** exist in the repo as:

`META/WORK-QUEUE-SYS.md`

This file is authoritative for:
- file order,
- status (`pending | merged | skipped | delta-check`),
- resume notes.

If chat state conflicts with repo queue, **repo queue wins** unless overridden.

### 5.3 “What’s next?” protocol
When you ask “What’s next?”, I must return:
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
Default: **exactly one SYS file per response**.

Multiple files only when explicitly requested.

### 6.2 File header (locked)
First line **must** be:
PATH: <relative/path>.md

### 6.3 Copy/paste safety (locked)
- Deliverable returned in **one fenced markdown block**
- No extra content inside the block

### 6.4 Density standard (locked)
Operator-grade only:
- decision rules,
- gates,
- failure signatures,
- transition logic.

No narrative filler.

---

## 7. Change Reporting (mandatory)

Every SYS update must include **outside the code block**:

### 7.1 Delta Summary
- **Added**
- **Modified**
- **Removed** (only if necessary)
- **Why** (usability / consistency / canonical map)

### 7.2 No silent deviations
Any deviation from:
- queue,
- structure,
- numbering,
- diagram rules  
must be explicitly declared and justified.

### 7.3 Conflicting instructionals
If instructionals disagree:
- preserve both as named variants,
- add a selection rule,
- never silently delete.

---

## 8. Systems Page Standard

### 8.1 Section numbering (locked)
SYS pages use numbered sections (`## 1. Purpose`, etc.).

Legacy structures are preserved unless you request migration.

### 8.2 Combined attack + defence rule (binding)
Default: SYS pages **combine attack and defence**.

Enforced by:
1. inserting a **Defence Model** section if missing,
2. integrating defence as **defender triggers → attacker responses**,
3. creating defence-only pages **only** when content is cross-hub reusable.

---

## 9. ASCII Diagram Standard

### 9.1 Requirement
At least one diagram per SYS page when it improves clarity.

### 9.2 Constraints (locked)
- ≤130 characters per line
- Plain triple-backtick fence only
- **No language tags**
- **No `~~~text` fences**

### 9.3 Conventions
- `[HUB]` = platform
- `(OUTCOME)` = finish / sweep / top
- `{OR}` = branch
- `!` = gate / failure

### 9.4 Broken diagram remediation
If a diagram renders incorrectly:
- next response reissues **diagram only**,
- include one-line fix note.

---

## 10. Delta Check Loop

After queue completion:
- verify instructional coverage,
- verify density,
- verify diagrams,
- verify links,
- verify attack + defence integration.

---

## 11. Decision Surfacing

Whenever a decision is required, I must state:
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
- **v0.5 (from v0.4)**
  - Added mandatory instructional lifecycle gate (TRN → BIO → VN → SYS).
  - Prohibited SYS merges without BIO + VN present in project files.
  - Added explicit SYS merge entry criteria and cross-project handoff rule.
  - Clarified VN role as non-canonical unless grounded or marked provisional.
  - Hardened batch-safe execution assumptions for SYS work.
  - Tightened queue authority and resume semantics.
  - Consolidated defence-integration rule as binding.

End — BOA-SYS v0.5
