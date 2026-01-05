PATH: BOA-SYS.md

# BITS Ops Agreement — SYS Merge Workflow (BOA-SYS) v0.3

## 0. Purpose (binding)
This agreement defines the **operational workflow** for merging multiple instructionals into **canonical SYS pages** in BITS (BJJ Instructional Teaching System).

It exists to prevent:
- duplicate system pages,
- low-signal “summary” content,
- uncontrolled drift from the agreed queue,
- and silent changes without a reason given.

This agreement governs **how we work**. It does not replace Kano Scroll (repo/training manual) nor Jigoro Text (BIO standard).

### 0.1 Draft vs Published (operating definitions)
- **Draft:** content not yet pasted into GitHub; may change rapidly.
- **Published:** content pasted into GitHub; treated as binding until the next version bump.

---

## 1. Scope and Boundaries

### 1.1 What this agreement governs
- SYS merge queue execution (file-by-file)
- Source intake rules (Project files vs pasted text)
- Output format rules (copy/paste safe)
- Change reporting requirements (“what changed and why” every time)
- Diagram rules (ASCII, width discipline)

### 1.2 What this agreement does *not* govern
- BIO report creation rules and Technique Library formatting (Jigoro Text governs)
- VN or session standards (Kano Scroll governs)
- New repo restructuring decisions unless explicitly requested

---

## 2. Canonical Principle (non-negotiable)
- `SYS/` is the **single merged system library**.
- If a topic already exists in `SYS/`, we **update that file** rather than creating a new duplicate.
- `INS/` holds per-instructional detail (BIO/VN/transcripts). SYS holds the merged durable system view.

---

## 3. Inputs and Source Hierarchy (how you give me material)

### 3.1 Preferred delivery method: Project files
Default preference: you add transcripts/BIO/VN as **project files** in ChatGPT.

Why:
- better persistence and retrieval versus long chat scroll
- reduces “where are we?” and “what did you base this on?” problems

### 3.2 Practical source hierarchy (default)
- **BIO + VN** = primary merge inputs (fast, high signal)
- **Transcripts** = audit layer (used selectively to add missed details or verify emphasis)

### 3.3 When transcripts are used (standard)
Transcripts are used:
- when BIO/VN quality is inconsistent or thin on a topic,
- when you explicitly request “extract more from transcript,”
- when we are building a **first canonical page** for a high-impact hub,
- during **delta checks** (see Section 9).

### 3.4 When transcripts are *not* deeply mined (standard)
If BIO/VN are strong and consistent, transcripts are used lightly:
- for spot-checking named concepts, rules, and failure signatures,
- for filling obvious gaps (e.g., a submission system that appears central but is thin in VN).

### 3.5 Transcript Retrieval Standard (long-text handling)
When transcripts are large, transcript use follows an explicit retrieval method so coverage is predictable.

#### 3.5.1 Default mode: Targeted extraction (fast)
Use when BIO/VN are acceptable.
- Search by **named entities** and **system keywords** (e.g., “toe hold”, “double trouble”, “leg lace”, “Achilles”, “cross ashi”).
- Pull only:
  - decision rules (IF/THEN),
  - named gates/constraints,
  - failure signatures + fixes,
  - and explicit transition triggers.
- Output impact: adds “operator detail” without rewriting the whole page.

#### 3.5.2 Deep mode: System-first sweep (slower, higher coverage)
Use when BIO/VN are weak, inconsistent, or you request max extraction.
- Sweep transcript by **module/chapters** where the system is taught.
- Capture:
  - full control model (what must be true),
  - full defence tree,
  - finishing mechanics cues,
  - and the drill progression if present.
- Output impact: significantly expands the SYS page.

#### 3.5.3 Delta mode: Gap + contradiction audit (post-merge)
Use during the delta check loop.
- Validate:
  - we didn’t miss a major branch/dilemma,
  - we didn’t contradict a core rule stated in transcript,
  - and the system’s “non-negotiables” match the instructional emphasis.
- Output impact: small but high-value corrections.

#### 3.5.4 Coverage declaration (required)
For any SYS update that uses transcripts, state in the delta summary:
- Mode used: Targeted / Deep / Delta
- Keywords/chapters used (short list)
- What new elements were added because of transcript (2–6 bullets)

#### 3.5.5 Practical limits (explicit)
- We do not attempt line-by-line extraction of an entire transcript unless you request it.
- Default objective is: extract **system logic**, not rewrite the transcript.

### 3.6 Source hooks (required when adding non-obvious content)
If new technical content is added (new rule, gate, branch, failure signature, mechanic, named concept):
- include at least one **source hook** in the update’s delta summary:
  - BIO reference and/or VN reference, and TRN reference only if TRN was used.

---

## 4. Queue Discipline (how we avoid veering off)

### 4.1 Single queue rule
- We maintain **one active working queue**.
- We execute **top-to-bottom**.
- We do not jump ahead unless you explicitly instruct.

### 4.2 “What’s next?” protocol
When you ask “What’s next?”, I must reply with:
- the **next file path** in the queue,
- whether it is **new** or **merge into existing**,
- and what you should paste next (or confirm is present as a project file).

### 4.3 Per-update queue position + status (required)
Every update response must state:
- Queue position: `#n / #N`
- Status of the current file: `merged | pending | skipped`
- If skipped: one-line reason + what is next.

### 4.4 If a file was already completed
If you suspect a file was already updated:
- I must state whether it is:
  - **already merged in this run**, or
  - **pending**, or
  - **needs delta check** (see Section 9).

---

## 5. Output Contract (format, density, and copy/paste safety)

### 5.1 One-file-per-response (locked)
- Output **exactly one file** per response unless you explicitly request otherwise.

### 5.2 File header (locked)
First line must be:
- `PATH: <relative/path>.md`

### 5.3 Copy/paste rule (locked)
- Deliverable is returned in **one fenced markdown code block**.
- No extra content inside that code block besides the file.

### 5.4 Density standard (locked)
Default density is **operator-grade**:
- procedural/conditional bullets
- explicit gates and failure signatures
- avoids narrative bloat
- no “filler” sections

---

## 6. Change Reporting (mandatory every update)
Every time I return an updated file, I must include **outside the code block**:

### 6.1 “Delta Summary” (required)
- **Added:** bullets / sections introduced
- **Modified:** meaningful changes to existing logic
- **Removed:** only if necessary; otherwise avoid deletions
- **Why:** short rationale tied to usability/consistency/canonical map

### 6.2 No silent deviations (required)
If I deviate from:
- the queue,
- the file structure,
- the numbering convention,
- or the diagram standard,
I must state **what deviated** and **why**.

### 6.3 Conflicts across instructionals (required handling)
If two instructionals conflict:
- preserve both as `Variant A / Variant B` (or named variants),
- add a **selection rule** (when to use A vs B),
- do not silently delete one.

---

## 7. Systems Page Standard (SYS files)

### 7.1 Section numbering (locked)
SYS pages use numbered sections:
- `## 1. Purpose`
- `## 2. When to Use It`
- etc.

(If a legacy file already uses a different structure, default is to preserve and migrate only when you request.)

### 7.2 Top outcomes in transitions (locked)
Transition pages must include links to:
- sweep-to-top / top outcomes,
when they naturally occur in the system.

---

## 8. ASCII Diagram Standard (mandatory)

### 8.1 Required placement
Include at least one diagram:
- typically as `## X. ASCII Control Map` or similar.

### 8.2 Diagram constraints (locked)
- Max **130 characters per line**
- Use a plain fenced block:
  - use ``` (no language tag)
- Must render as an “actual diagram” (boxes/arrows), not a loose sketch.

### 8.3 ASCII conventions
Recommended:
- `[HUB]` = positional platform
- `(OUTCOME)` = finish/sweep/top/reset
- `{OR}` = branch
- `!` = gate/fail condition

### 8.4 If a diagram renders broken (required remediation)
- Next response must reissue the diagram **alone**, plus a one-line note stating what was fixed.

---

## 9. Delta Check Loop (post-merge audit)
After completing the queue, we run a **delta check** pass:

### 9.1 Delta check objectives
- confirm each SYS file reflects:
  - the merged content from the intended instructionals,
  - the operator-grade density target,
  - diagram compliance,
  - and internal link hygiene.

### 9.2 Delta check inputs
Use:
- BIO/VN as primary,
- transcripts for spot verification and gap filling.

---

## 10. Decisions You Control (and how I surface them)

### 10.1 Decision surfacing rule
Whenever a decision is required, I must state:
- the decision,
- why it matters,
- the default recommendation,
- and the alternative(s).

Examples:
- whether to create a new canonical page vs append into existing
- filename choice for a new hub page (e.g., `50-50-hub.md`)
- whether to refactor a legacy file into numbered sections

### 10.2 Blockers (required)
If work is blocked, I must state:
- what is blocked,
- what minimal decision/input unblocks it,
- what file in the queue can proceed next (if any).

---

## 11. Working cadence (practical)
- You paste the current SYS file (or confirm it exists as a project file).
- I return:
  1) merged SYS content (one file),
  2) delta summary (outside the code block),
  3) “Next:” the next file path in queue.

---

## 12. Versioning and changelog (locked)
- Any Published change requires a version bump (v0.2 → v0.3 → v0.4 …).
- Every version must include a short changelog summarising operational differences.

---

End — BOA-SYS v0.3
