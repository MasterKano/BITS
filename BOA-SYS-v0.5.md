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
