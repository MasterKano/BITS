PATH: BOA-SYS-v1.2.md

# BITS Ops Agreement — SYS Merge Workflow (BOA-SYS) v1.2

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
- You upload transcripts (TRN) only.
- VN and BIO are produced from TRN inside the project workflow, then promoted into SYS.

### 0.2 Pipeline (canonical)
**TRN → VN → BIO → SYS**

This agreement governs the **SYS phase** and the controls required to keep SYS canonical, deduplicated, and operator-grade.

---

## 1. Scope and Boundaries

### 1.1 What this agreement governs
- SYS merge queue execution (file-by-file)
- Instructional → SYS handoff rules
- Source intake rules (Project files vs pasted text)
- Output contract (copy/paste safe)
- Change reporting requirements (“what changed and why” every time)
- Diagram rules (ASCII, width discipline; fencing per Kano)
- Defence integration rule (attack + defence combined in SYS by default)
- Training games/drills inclusion policy and formatting
- SYS page build standard and enforcement cadence
- Best-version enforcement (two-pass delivery) for each SYS item

### 1.2 What this agreement does not govern
- VN or session standards (Kano governs)
- BIO report creation rules and formatting (Jigoro governs)
- Repo restructuring unless explicitly requested

---

## 2. Canonical Principle (non-negotiable)
- `SYS/` is the **single merged system library**.
- If a topic already exists in `SYS/`, **update the existing file** rather than creating a duplicate.
- `INS/` holds instructional-specific artifacts (TRN/VN/BIO).
- `SYS/` holds the durable, merged, instructional-agnostic system view.

---

## 3. Instructional Lifecycle Gate (binding)

### 3.1 Mandatory lifecycle order
SYS merge may not begin for an instructional until the following are complete:
1. TRN intake (source-of-truth)
2. VN generated (Titles-aligned when Titles file exists)
3. BIO generated (template-locked per Jigoro)
4. SYS merge (this agreement)
5. Delta check
6. Queue advancement

Skipping steps 2 or 3 is not permitted unless explicitly instructed.

### 3.2 SYS merge entry criteria (gate)
Before SYS merge starts, the following must exist in project files or be pasted in chat:
- BIO file (`INS/.../BIO/BIO.md` or equivalent)
- VN files (`INS/.../VN/VN01..VN0N`, or declared partial scope)

If only TRN exists, generate VN and BIO first (Kano/Jigoro), then begin SYS.

---

## 4. Inputs and Source Hierarchy

### 4.1 Source hierarchy (binding)
- **VN + BIO** = primary SYS merge inputs
- **TRN** = source-of-truth and audit layer (resolve ambiguity/conflict)

### 4.2 Source-of-truth rule (binding)
If VN/BIO conflicts with TRN, SYS must follow TRN.

### 4.3 Transcript retrieval modes (declared)
For any SYS update using TRN, one mode must be stated in the delta summary:
- **Targeted (default):** keyword + concept pulls only
- **Deep:** system-first sweep (explicitly requested or required for first-time canonical build)
- **Delta:** contradiction/gap audit after merge

### 4.4 Provenance floor (non-negotiable)
Any non-obvious new technical content must be grounded in at least one of:
- BIO reference, and/or
- TRN reference (if TRN used)

---

## 5. Queue Discipline

### 5.1 Single queue rule
- One active SYS queue.
- Executed top-to-bottom.
- No jumping unless explicitly instructed.

### 5.2 Queue artifact (binding)
The queue must exist in the repo as the authoritative queue file and include:
- file order
- status (`pending | merged | skipped | delta-check`)
- resume notes

### 5.3 Per-response status (required)
Every SYS response must state outside the copy box:
- item number (`n/N`)
- action (`CREATE` or `UPDATE`)
- what changed (1–3 bullets)
- next item

### 5.4 Best-Version Declaration (required)
Each SYS delivery must declare one:
- **Pass 1 (compliant draft)**, or
- **Pass 2 (best version)**

Queue cannot advance past an item until a **Pass 2** is delivered unless the user explicitly waives Pass 2.

---

## 6. Output Contract (locked)

### 6.1 One file per response (default)
- One file per response by default.
- Multiple files only when explicitly requested.

### 6.2 File header (locked)
First line inside the block:
`PATH: ...`

### 6.3 Copy/paste safety (locked)
- Entire file delivered in one fenced markdown block.
- No partial outputs.

### 6.4 Best-Version Pass (binding)
For each SYS item, perform two passes unless the user explicitly requests otherwise:
- **Pass 1:** compliant operational draft (meets Section 8 requirements).
- **Pass 2:** best-version refinement: add missing operator-grade layers (routing heuristics, defaults, failure diagnostics, interface tags, and training cards where beneficial) and remove redundancy.

Queue advances only after Pass 2 is delivered (or user explicitly waives Pass 2).

---

## 7. Change Reporting (mandatory)

Outside the code block, every SYS update includes:
- **Added**
- **Modified**
- **Removed** (only if necessary)
- **Why**
- **Sources touched** (INS paths used)

No silent deviations.

### 7.1 No Regression Rule (binding)
Revisions may compress wording but must not remove operator-grade capabilities (gates, defaults, chain logic, routing, governance, or mandatory sections) unless explicitly requested.

If removal occurs, list Removed items in the delta summary.

---

## 8. Systems Page Standard (binding)

### 8.1 Operator-grade density (locked)
SYS pages must be operator-grade:
- decision rules
- gates
- outputs/success criteria
- transition logic
- opponent reactions → responses
- failure signatures → fixes

No narrative filler.

### 8.2 Required section order (default; upgraded in v1.2)
Unless content type makes a section irrelevant, SYS pages follow this order:

1) **Purpose**  
2) **Inputs / Preconditions** (if applicable)  
3) **Outputs / Success Criteria**  
4) **Core Model / Engine**  
5) **Gates (override rules)**  

6) **Top-6 Situations Playbook** (mandatory unless truly inapplicable; see 8.2A)  

7) **Opponent Reactions → Responses**  
8) **Failure Signatures → Fix**  

9) **Trigger Recognition Checklist** (mandatory when the system includes a commitment threshold; see 8.2B)  
10) **Quality / Capture Checklist** (mandatory when the system claims capture/control/handle; see 8.2C)  

11) **Interfaces** (routing rules; see 8.4)  
12) **Diagram (ASCII)**  
13) **Drills and Games** (when beneficial; per Section 9)

If a section is not applicable, omit it—do not pad.

#### 8.2A Top-6 Situations Playbook (mandatory)
Every SYS page must include a Top-6 Situations Playbook unless it is purely taxonomic/reference.

Format:
- Situation → Default response → Win condition/state change target

Minimum:
- 6 situations
- at least 2 situations must cover opponent escalation (pressure/retreat/strip/angle)

If omitted:
- permitted only when the page is a taxonomy/reference node; must be explicit in delta summary (“Playbook omitted: reference node”).

#### 8.2B Trigger Recognition Checklist (mandatory when commitments exist)
If the system contains any of the following, a Trigger Recognition Checklist is required:
- going underneath/rotational commitments
- inversion/entry commitments
- exposure/finish commitments
- any “permission cue” claim (e.g., “only commit when…”)

Format:
- 3–7 binary cues
- a fail-safe line: “If cues are not present, do NOT commit; return to <safer action>.”

If omitted:
- only if there is no commitment threshold in the system; must be explicit in delta summary.

#### 8.2C Quality / Capture Checklist (mandatory when captures/controls exist)
If the system claims a capture/control/handle/connection/pin, include a Quality/Capture Checklist.

Format:
- 4–8 durability checks (survives step, strip, angle, pressure beat)
- include one fail-fast downgrade rule: “If X fails, downgrade to Y.”

If omitted:
- only if the system has no capture state; must be explicit in delta summary.

### 8.3 Controller page add-ons (mandatory when the page is a controller)

**A) Domain Progression Chain Table** (compact)  
A controller page must define the ordered progression chain that governs the domain (i.e., the requirements sequence the opponent/system is building).

- The chain must be domain-appropriate (examples: passing chain, clinch chain, takedown chain, leglock control chain, back-take chain).
- For each link: include “What you read” + “What you deny” (one line each).
- Purpose: fast diagnosis and early denial of the current link before the next link is enabled.

**B) Gate Default Actions**  
Each gate must include a “Default action” line that is executable (not conceptual).
Example form:
- **Default action:** frame high/low + turn-to-side + shrimp → rebuild barriers

### 8.4 Interfaces rule (anti-sprawl; upgraded to routing rules)
Every SYS page must list:
- what it depends on (upstream selectors/gates), and
- what it feeds (downstream hubs/entries/finishes)

Each interface entry must be a routing rule with a one-line use-when tag.

Required format:
- **If <condition/state>, go to `<file.md>` — use when: <trigger/context>.**

Minimum set:
- at least 1 upstream (“how you arrive here”)
- at least 1 downstream (“where you go next”)
- at least 1 defensive diversion (“if threatened/pressure/hip-line then…”)

### 8.5 Diagrams (binding; delegated to Kano)
Diagram constraints and fencing are governed by the current Kano Scroll.
SYS pages comply with Kano’s:
- ASCII-only
- ≤120 characters per line
- fence style requirements

### 8.6 Controller Completeness Checklist (binding)
If a SYS page is a controller/decision layer, it must include:
- domain progression chain table (read/deny per link),
- gate default actions (executable),
- selector pack (short rules) OR explicit link-outs with a 1-line in-page summary,
- exit governance (reset denial rules) when the opponent’s primary defense is reset,
- game cards when the controller requires recognition + switching to acquire.

---

## 9. Drills and Games (binding)

### 9.1 When included
Where beneficial, SYS pages include a final section titled:
`## Drills and Games`

Include when it materially improves acquisition/testing, especially for:
- decision models (recognition + switching)
- governance modules (anti-exit, constraints, cycle-break)
- retention engines (orientation, framing layers)
- hubs where stabilization + exit denial are core skills

Optional where it adds noise (pure taxonomy/reference nodes).

### 9.2 Game Card format (mandatory when games are included)
Games must be practical; no callouts required.

Each game uses this exact card:

- **Start:** (explicit starting position/state)  
- **Defender wins:** (clear measurable condition)  
- **Passer wins:** (clear measurable condition)  
- **Rules:** (1–3 constraints that force the intended behavior)  
- **Reset:** (exact reset triggers)  
- **Rounds:** (time or reps, plus switch instruction)

### 9.3 Training Clarity Standard (binding)
When drills/games are included, they must be runnable without interpretation:
Start / Defender wins / Passer wins / Rules / Reset / Rounds.

No callouts required unless the user asks for them. Use standardized scoring vocabulary where possible.

### 9.4 Scoring vocabulary (standardize terms)
Use a small consistent vocabulary across games to reduce re-reading:
- **Outside knee line**
- **Hip line touch**
- **Pin**
- **Disengage to two steps**
- **Hold for 3 seconds**
- **Timer (20s / 15s)**

### 9.5 Provenance constraint
Drills/games may extend training design beyond the instructional, but must not introduce new mechanical claims. They operationalize the mechanics already defined in the page.

---

## 10. Combined Attack + Defence Rule (binding)
Default: SYS pages combine attack + defence by default.
Enforced by:
1. inserting a Defence Model section if missing,
2. integrating defence as defender triggers → attacker responses,
3. creating defence-only pages only when content is cross-hub reusable and clearly separable.

---

## 11. Consistency Enforcement (binding)

### 11.1 Every-5-item delta consistency check
Every 5 SYS items, run a consistency check for:
- terminology consistency (domain-specific core terms)
- section order compliance
- controller add-ons present where required (domain chain table; gate default actions; completeness checklist)
- Top-6 Situations Playbook present where required
- Trigger checklist present where required
- Quality/Capture checklist present where required
- interface routing rules present (If X, go to Y format)
- diagram compliance with Kano
- game cards follow the required format and vocabulary
- no duplicate systems created

### 11.2 Fix-before-advance rule
If any violation is detected, fix immediately before advancing the queue.

---

## 12. Versioning and Changelog (locked)
Every published change requires a version bump.

### 12.1 Changelog
- **v1.2 (from v1.1)**
  - Added Top-6 Situations Playbook requirement (Section 8.2A) and inserted into required section order.
  - Added Trigger Recognition Checklist requirement for commitment-based systems (Section 8.2B).
  - Added Quality/Capture Checklist requirement for capture/control/handle systems (Section 8.2C).
  - Upgraded Interfaces rule to routing rules: “If X, go to file.md — use when …” with minimum upstream/downstream/defensive set (Section 8.4).
  - Updated Every-5-item consistency check to enforce the above additions (Section 11.1).

End — BOA-SYS v1.2