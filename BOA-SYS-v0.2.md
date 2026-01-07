PATH: BOA-SYS.md

# BITS Ops Agreement — SYS Merge Workflow (BOA-SYS) v0.4

## 0. Purpose (binding)
This agreement defines the operational workflow for merging multiple instructionals into canonical SYS pages in BITS.

It exists to prevent:
- duplicate system pages,
- low-signal “summary” content,
- uncontrolled drift from the agreed queue,
- silent changes without a reason given,
- and SYS pages that exclude defence logic when defence instructionals are merged.

This agreement governs how we work. It does not replace Kano Scroll (repo/training manual) nor Jigoro Text (BIO standard).

### 0.1 Draft vs Published (operating definitions)
- Draft: content not yet pasted into GitHub; may change rapidly.
- Published: content pasted into GitHub; treated as binding until the next version bump.

---

## 1. Scope and Boundaries

### 1.1 What this agreement governs
- SYS merge queue execution (file-by-file)
- Source intake rules (Project files vs pasted text)
- Output format rules (copy/paste safe)
- Change reporting requirements (“what changed and why” every time)
- Diagram rules (ASCII, width discipline)
- Defence integration rule (attack + defence combined in SYS by default)

### 1.2 What this agreement does not govern
- BIO report creation rules and Technique Library formatting (Jigoro Text governs)
- VN or session standards (Kano Scroll governs)
- New repo restructuring decisions unless explicitly requested

---

## 2. Canonical Principle (non-negotiable)
- SYS/ is the single merged system library.
- If a topic already exists in SYS/, we update that file rather than creating a new duplicate.
- INS/ holds per-instructional detail (BIO/VN/transcripts). SYS holds the merged durable system view.

---

## 3. Inputs and Source Hierarchy (how you give me material)

### 3.1 Preferred delivery method: Project files
Default preference: you add transcripts/BIO/VN as project files in ChatGPT.

Why:
- better persistence and retrieval versus long chat scroll
- reduces “where are we?” and “what did you base this on?” problems

### 3.2 Practical source hierarchy (default)
- BIO + VN = primary merge inputs (fast, high signal)
- Transcripts = audit layer (used selectively to add missed details or verify emphasis)

### 3.3 When transcripts are used (standard)
Transcripts are used:
- when BIO/VN quality is inconsistent or thin on a topic,
- when you explicitly request “extract more from transcript,”
- when we are building a first canonical page for a high-impact hub,
- during delta checks (see Section 9).

### 3.4 When transcripts are not deeply mined (standard)
If BIO/VN are strong and consistent, transcripts are used lightly:
- for spot-checking named concepts, rules, and failure signatures,
- for filling obvious gaps (e.g., a submission system that appears central but is thin in VN).

### 3.5 Transcript Retrieval Standard (long-text handling)
When transcripts are large, transcript use follows an explicit retrieval method so coverage is predictable.

#### 3.5.1 Default mode: Targeted extraction (fast)
Use when BIO/VN are acceptable.
- Search by named entities and system keywords (e.g., “toe hold”, “double trouble”, “leg lace”, “Achilles”, “cross ashi”).
- Pull only:
  - decision rules (IF/THEN),
  - named gates/constraints,
  - failure signatures + fixes,
  - explicit transition triggers.
- Output impact: adds operator detail without rewriting the whole page.

#### 3.5.2 Deep mode: System-first sweep (slower, higher coverage)
Use when BIO/VN are weak, inconsistent, or you request max extraction.
- Sweep transcript by modules/chapters where the system is taught.
- Capture:
  - full control model (what must be true),
  - full defence tree,
  - finishing mechanics cues,
  - drill progression if present.

#### 3.5.3 Delta mode: Gap + contradiction audit (post-merge)
Use during the delta check loop.
- Validate:
  - no major branch/dilemma was missed,
  - no core transcript rule was contradicted,
  - the system’s non-negotiables match instructional emphasis.

#### 3.5.4 Coverage declaration (required)
For any SYS update that uses transcripts, state in the delta summary:
- Mode used: Targeted / Deep / Delta
- Keywords/chapters used (short list)
- What new elements were added because of transcript (2–6 bullets)

#### 3.5.5 Practical limits (explicit)
- We do not attempt line-by-line extraction of an entire transcript unless requested.
- Default objective is: extract system logic, not rewrite the transcript.

### 3.6 Source floor (provenance requirement)
For SYS merges, any non-obvious new technical content (new rule, gate, branch, failure signature, mechanic, named concept) must be grounded in at least one of:
- BIO reference, and/or
- TRN reference (only if TRN was used).

VN may be used as an operator synthesis layer, but VN-only additions are not treated as canonical unless explicitly marked as provisional by user request.

---

## 4. Queue Discipline (how we avoid veering off)

### 4.1 Single queue rule
- We maintain one active working queue.
- We execute top-to-bottom.
- We do not jump ahead unless you explicitly instruct.

### 4.2 Queue artifact (binding)
The working queue must be stored in the repo as:

- `META/WORK-QUEUE-SYS.md`

This file is authoritative for:
- the ordered list of SYS files to process,
- the current status per file (pending | merged | skipped | delta-check),
- and notes required to resume in a new chat.

If a queue exists in chat and conflicts with `META/WORK-QUEUE-SYS.md`, the repo queue wins unless you explicitly override it.

### 4.3 “What’s next?” protocol
When you ask “What’s next?”, I must reply with:
- the next file path in the queue,
- whether it is new or merge into existing,
- what you should paste next (or confirm exists as a project file).

### 4.4 Per-update queue position + status (required)
Every update response must state:
- Queue position: #n / #N
- Status of the current file: merged | pending | skipped | delta-check
- If skipped: one-line reason + what is next.

### 4.5 If a file was already completed
If you suspect a file was already updated:
- I must state whether it is:
  - already merged in this run, or
  - pending, or
  - needs delta check (see Section 9).

---

## 5. Output Contract (format, density, and copy/paste safety)

### 5.1 One-file-per-response (default)
Default: output exactly one file per response unless you explicitly request multiple files in one response.

### 5.2 File header (locked)
First line must be:
- `PATH: <relative/path>.md`

### 5.3 Copy/paste rule (locked)
- Deliverable is returned in one fenced markdown code block.
- No extra content inside that code block besides the file.

### 5.4 Density standard (locked)
Default density is operator-grade:
- procedural/conditional bullets
- explicit gates and failure signatures
- avoids narrative bloat
- no filler sections

---

## 6. Change Reporting (mandatory every update)
Every time I return an updated file, I must include outside the code block:

### 6.1 Delta Summary (required)
- Added: bullets/sections introduced
- Modified: meaningful changes to existing logic
- Removed: only if necessary; otherwise avoid deletions
- Why: short rationale tied to usability/consistency/canonical map

### 6.2 No silent deviations (required)
If I deviate from:
- the queue,
- the file structure,
- the numbering convention,
- or the diagram standard,
I must state what deviated and why.

### 6.3 Conflicts across instructionals (required handling)
If two instructionals conflict:
- preserve both as Variant A / Variant B (or named variants),
- add a selection rule (when to use A vs B),
- do not silently delete one.

---

## 7. Systems Page Standard (SYS files)

### 7.1 Section numbering (locked)
SYS pages use numbered sections:
- `## 1. Purpose`
- `## 2. When to Use It`
- etc.

If a legacy file uses a different structure, default is to preserve and migrate only when you request.

### 7.2 Top outcomes in transitions (locked)
Transition pages must include links to sweep-to-top / top outcomes when they naturally occur in the system.

### 7.3 Combined attack + defence rule (binding)
Default: SYS pages are combined attack + defence.

I will enforce this in merges by:
1) inserting a “Defence Model” section if missing, and/or
2) integrating defence instructional material as:
   - defender triggers → attacker responses,
3) creating defence-only pages only when the content is clearly reusable across many hubs (cross-hub defence principles), not specific to a single hub.

---

## 8. ASCII Diagram Standard (mandatory)

### 8.1 Required placement
Include at least one diagram, typically as “ASCII Control Map” or similar.

### 8.2 Diagram constraints (locked)
- Max 130 characters per line
- Use a plain fenced block with triple backticks only (no language tag).
- Do not use fences like “```text” or “~~~text”.

Example (fence format only; content is illustrative):
