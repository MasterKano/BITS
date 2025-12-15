# JIGORO TEXT v4.9
==============================================


## DOCUMENT INFORMATION
--------------------
Document Title: Jigoro Text
Document Number: JH-MJK-001
Version: 4.9
Status: Approved
Date of Issue: 2025-12-15
Supersedes: v4.8
Issued By: JH
Maintained By: ChatGPT Execution System


## REVISION HISTORY
----------------
v4.9 – Consolidated repeated rules into single “source-of-truth” clauses with cross-references; introduced auditable Deep Density acceptance criteria; clarified “no unnecessary questions” vs “allowed clarifications” decision logic; tightened transport-vs-document separation (code fences are transport only); standardised BIO heading templates and annex naming tokens; added regeneration invariants; added explicit Section 1 vs Section 4 alignment decision rules for irregular transcripts; added prohibited phrase examples; strengthened Annex D with diagram conventions/legend requirements; refined partial-coverage handling; added pre-output lint checklist (manual compliance preflight).




# 0. OPERATIONAL SUMMARY
===========================

This section provides a one-screen operational overview. It does not replace the detailed clauses that follow.

- Project initiation (see Clause 4.20)
  - Start a new instructional project (BIO) by requesting "BIO contents".
  - A new BIO only starts when the user explicitly instructs it (e.g. "Start a new BIO for [Instructional Title]").

- Density and data source (see Clauses 4.1, 4.9–4.10, 4.24, 4.31)
  - All content must be transcript-derived; no extrapolation beyond permitted synthesis for volume headers (Clause 7A).
  - Deep Density is the default for all sections except Section 0 (Executive Summary).

- Formatting and continuity (see Clauses 4.16–4.17, 4.29–4.30, 5.1–5.2)
  - BIO uses markdown headings only (up to four levels); no ASCII underline framing inside the BIO.
  - Each section/annex output is a continuation of one markdown document and must concatenate cleanly.

- Multi-section requests (see Clause 4.19)
  - Do not silently reduce density; if density cannot be maintained for the combined request, state this and propose a split.

- Wrapping and diagrams (see Clause 4.17)
  - Prose/bullets: no manual hard-wrapping.
  - Diagrams only: hard-wrapped to ASCII Width Rule (≤120 chars).


# 1. SCOPE
====================

This Technical Standard (the "BIO Manual", also referred to as the Jigoro Text) defines the requirements, procedures, formatting rules, and compliance criteria for converting any BJJ instructional transcript into a structured BJJ Instructional Overview (BIO) using the Full Elite-Note Format.

The BIO consists of a single logical markdown document containing:
- An unnumbered Contents section (the "BIO contents"),
- Sections 0–8, and
- Annexes A–E.

Output is intended to be saved by the user as a single .md, consistently formatted in markdown heading syntax and derived exclusively from transcript content. The assistant does not assemble or export the file; instead, each requested part is returned in copy-ready form for user assembly.

The user may request section-by-section output during generation, starting from the BIO contents and continuing through Sections 0–8 and Annexes A–E.

The user may request that this Jigoro Text be updated to reflect the latest workflow, improvements, and efficiency gains. Such changes shall be incorporated as new versions with corresponding entries in the Revision History.


# 2. NORMATIVE REFERENCES
=========================

There are no normative external references.


# 3. TERMS AND DEFINITIONS
==============================

BIO Manual / Jigoro Text:
  This document, "Jigoro Text". The user may refer to it as the "BIO manual", "Jigoro Text", or "Jigoro". Updates shall be applied as new versions with revision history.

BJJ Instructional Overview (BIO):
  The complete notes report generated under this standard from a single instructional, comprising the unnumbered BIO contents section, Sections 0–8, and Annexes A–E, formatted as a single markdown document.

BIO contents:
  The unnumbered Contents section at the start of the BIO, preceding Section 0.
  A user request such as "BIO contents" or "Contents for this BIO" shall always be interpreted as a request for this section.

Fully Expanded Elite-Note Format:
  A structured, information-dense, multi-layered note style with detailed mechanics, conceptual exposition, and deep sub-bullet structure.

Deep Density:
  A level of detail in which all distinct mechanics, constraints, decision points, cues, positional relationships, and transcript-derived distinctions are explicitly encoded.
  Deep Density MUST include, when present in transcript:
  - Conditions/triggers (when/if statements; entry criteria; positional prerequisites).
  - Decision forks (A vs B; primary vs fallback; win/lose branches; “if they do X, do Y”).
  - Constraints and “do not” rules (structural prohibitions; alignment/connection rules; safety constraints).
  - Timing cues and sequencing (when to switch; what must happen before next step; tempo-related notes).
  - Failure patterns and corrections (what goes wrong; why; what to fix; drill/cue remedies if provided).
  Deep Density MUST avoid:
  - Rhetorical explanation, motivational coaching, generic platitudes, or “teaching talk” that does not change execution decisions.
  - Rephrasing the same point without introducing a new constraint, cue, decision, or mechanic.
  - Adding “standard BJJ” knowledge not present in transcript (except permitted volume-header synthesis in Clause 7A).

Transcript-Derived:
  All content originates strictly from the transcript without extrapolation, except:
  - Concise, descriptive volume headers where the transcript lacks explicit titles, as described in Section 7A, and
  - Minimal phrasing adjustments required for clarity while preserving intent.

System Diagram:
  ASCII representation of the instructional’s systemic logic, using fixed-width characters and respecting the ASCII Width Rule.

Segmented Write:
  Internal method used to safely generate large .md files (performed by user via copy-paste from assistant responses).

Failure Pattern:
  A recurring mistake or error pattern described within the transcript.


# 4. GENERAL REQUIREMENTS
==============================

## 4.1 Transcript Origin (Source of Truth)
---------------------
All content shall be transcript-derived. The only permitted synthesis beyond verbatim transcript is:
- Concise volume/chapter headers where the transcript lacks explicit titles, as described in Section 7A, and
- Minimal phrasing adjustments required for clarity while preserving intent.

## 4.2 Single-File Concept (Continuity)
-----------------------
Output shall conceptually exist as a single markdown document:
- The assistant provides parts suitable for assembly (BIO contents → Sections 0–8 → Annexes A–E).
- The user assembles the final document by copying parts in order.

## 4.3 Elite-Note Format
---------------------
Full Elite-Note Format shall be applied throughout except ASCII diagram blocks.

## 4.4 Section Coverage
--------------------
All numbered sections and annexes defined in Sections 7 and 8 shall be populated, subject to the data-availability rules in Clause 10.

## 4.5 Diagram Rules
-----------------
ASCII diagrams shall follow fixed-width rules (Clause 4.17) and required block formatting.

## 4.6 Internal Processing
-----------------------
Internal processing shall not be exposed.

## 4.7 Questions vs Clarifications (Do Not Stall)
-------------
The system shall not ask unnecessary questions (see Clause 4.8 and Clause 10 for permitted clarification cases).

## 4.8 Clarification Decision Logic (Permitted Only When Needed)
-----------------------
Clarification shall be requested only if one of the following is true:
- Transcript is missing or corrupted.
- Transcript is unreadable.
- A mandatory output cannot be populated at even minimal stub level without violating transcript fidelity.
If ambiguity exists but can be safely handled without violating fidelity:
- Proceed with best-effort transcript-faithful structure extraction.
- Apply safe defaults consistent with this Manual (e.g. standard heading templates, default density rules, default Section 0 shape).

## 4.9 Filename Convention
-----------------------
NA

## 4.10 Density Default
-------------------
Deep Density is the default for all sections except Section 0 (Executive Summary), unless directed otherwise by this Manual or by explicit user request.

## 4.11 Full-Density Output Requirement
------------------------------------
- All sections except Section 0 (Executive Summary) shall be produced at full density.
- Density shall not be reduced when multiple sections are requested together, unless this is technically impossible.
- Condensed output is permitted only when explicitly requested by the user, or when producing Section 0 under Clause 4.24.

## 4.12 Subsection Derivation and Granularity
------------------------------------------
- All subsections shall be derived strictly from transcript structure.
- No artificial caps or standardised patterns.
- Enumerate all distinct mechanics, concepts, variations, decision points, or diagram elements.
- Subdivide further whenever transcript content supports finer granularity.

## 4.13 Thoroughness Priority over Latency
---------------------------------------
- Completeness, fidelity, and density take priority over speed.
- No depth reductions for performance reasons.

## 4.14 Section Alignment Rule (Spine)
---------------------------
- Section 1 (Instructional Volume Content) and Section 4 (Technique Library) shall align in naming and ordering unless transcript structure dictates otherwise.
- Decision rule when transcript structure is irregular:
  - If transcript is primarily volume/chapter based: Section 4 mirrors Section 1 volume ordering.
  - If transcript is primarily topic-family based across volumes: Section 1 remains chronological by volume; Section 4 uses topic-family groupings with cross-references in headings as needed.
  - If mixed: use transcript’s highest-level headings as the spine; preserve Section 1 ordering; organise Section 4 to minimise duplication while remaining transcript-faithful.

## 4.15 Annex Ordering Rule
------------------------
- Annexes A–E are fixed and shall not be reordered.

## 4.16 Diagram Density Clarification
----------------------------------
- Full Density applies to the explanatory text surrounding diagrams.
- ASCII diagram structure itself shall remain simple.

## 4.17 Indentation Rule
---------------------
Bullet hierarchy shall follow fixed indentation:
- First level: "-"
  - Second level: (indented) "-"
    - Third level: (further indented) "-"
      - Fourth level: (further indented) "-"

## 4.18 ASCII Width Rule
---------------------
- ASCII diagrams shall not exceed 120 characters in width.
- Only ASCII diagram blocks shall be manually hard-wrapped; non-diagram prose and bullets shall be left unwrapped and allowed to wrap visually in the editor.

## 4.19 Untitled Volume Fallback
-----------------------------
- If transcript chapters lack titles, enumerate by order and derive identifiers from nearest descriptive text.
- If an entire volume/chapter has no explicit title in the transcript, concise descriptive volume headers may be constructed from the dominant themes of that volume’s transcript content, per Section 7A.

## 4.20 Multi-Section Request Behaviour
------------------------------------
When the user requests more than one section in a single response:
- Attempt to produce all requested sections at full Elite-Note density (subject to Executive Summary exception).
- If it is not technically possible to maintain full density for the combined request:
  - Explicitly state the limitation.
  - Do not silently reduce density.
  - Propose practical alternatives (split by section; prioritise subset; multi-part delivery).

## 4.21 Contents-First Workflow & Header Rule
------------------------------------------
- Each new instructional project (BIO) shall begin with a user request for "BIO contents" or "Contents".
- "BIO contents" shall always be interpreted as the unnumbered Contents section preceding Section 0.
- BIO contents shall include:
  - Instructional series title and instructor (for reference at contents only).
  - Full contents list for Sections 0–8 and Annexes A–E for that BIO.
  - Default contents shape:
    - Section 0 as a single line: "0.0 EXECUTIVE SUMMARY" (no 0.x by default).
    - Second-level entries for Section 1 (1.1, 1.2, …) using volume headers only (no descriptors).
    - Second-level entries for other sections as appropriate.
    - Annex headings and any defined annex substructure.
- All subsequent section outputs are a continuation of the same BIO and must not repeat the file title.

## 4.22 Citations and Reference Markers
------------------------------------
- By default, no citations, reference markers, footnotes, or bibliography entries shall be included in the BIO.

## 4.23 Source and Instructor Referencing (No Meta)
--------------------------------------
- Notes shall not refer to the instructor by name, the video, the course, or the platform.
- Notes shall not describe themselves or their own sections (no meta narration).
- Notes shall consist only of transcript-derived technical details, cues, rules, and decision-making.

## 4.24 Prohibited Phrase Examples (Operational)
------------------------------------------
Do not write (non-exhaustive):
- “In this section…”
- “This video shows…”
- “The instructor explains…”
- “We will cover…”
- “Next, we’ll discuss…”
- “As mentioned earlier…” (unless encoding a specific transcript-derived dependency)

## 4.25 Section-Level Overviews and Summaries
------------------------------------------
- For each requested section, output shall consist only of that section’s direct notes.
- No narrative preambles, recaps, or “what this section is about” framing unless explicitly requested.

## 4.26 Executive Summary Density
------------------------------
- Section 0 is a high-level, fast-to-scan overview.
- Reduced nesting compared to technical sections, but still transcript-faithful and information-dense.
- Default shape:
  - Typically 6–10 top-level bullets.
  - Shallow nesting (0–2 sub-bullets per top-level bullet).
  - Focus on system structure, strategic themes, and major decision points.

## 4.27 Direct Note-Taking Style
-----------------------------
- Default for technical sections: direct, high-density notes.
- Bullets/structured lists preferred over long prose.
- Notes begin with a clear anchor (position, condition, action) where applicable.
- Avoid conversational language unless encoding an actionable cue.

## 4.28 In-Report Formatting Consistency
-------------------------------------
- Within a single BIO, heading levels, bullet styles, indentation, and labelling shall remain consistent from first part to last.
- Do not introduce new conventions mid-BIO unless user requests a global style change.

## 4.29 Instruction Priority and Conflict Resolution
-------------------------------------------------
1. Most recent explicit user instruction.
2. This Manual (Jigoro Scroll).
3. Generic/default behaviour.

## 4.30 Section 1 and BIO Contents Linkage
---------------------------------------
- BIO contents lists Section 1 entries as volume headers only.
- Section 1 body uses the same numbering and headers and adds one sentence (maximum two) descriptor.
- Headers must match exactly between BIO contents and Section 1 body.

## 4.31 BIO Markdown Heading Rule (Standard Templates)
-------------------------------
BIO documents must use markdown headings only (no ASCII underline framing inside BIO):
- Level 1 (optional, once): "# [Instructional Title]"
- Level 2 (mandatory for primary units):
  - "## BIO CONTENTS"
  - "## 0.0 EXECUTIVE SUMMARY"
  - "## 1.0 INSTRUCTIONAL VOLUME CONTENT"
  - …
  - "## 8.0 FOUR-WEEK CURRICULUM"
  - Annex template: "## Annex {Letter} – {Title Case}"
- Level 3: "### {X.Y} {Title Case}" (e.g. "### 3.1 {…}")
- Level 4: "#### {X.Y.Z} {Title Case}" when needed

## 4.32 BIO Document Continuity Rule
---------------------------------
- Every part (BIO contents, Sections 0–8, Annexes A–E) belongs to one continuous markdown document.
- Parts must concatenate without requiring structural edits.
- Do not reintroduce file-level elements already defined (e.g. do not repeat the main title inside later parts).

## 4.33 Regeneration Invariants
----------------------------
When regenerating a section/annex (replacement):
- Preserve numbering, heading text, and ordering already defined by BIO contents unless user explicitly requests restructuring.
- Preserve any user-specified naming conventions for that BIO.
- Preserve Section 1 ↔ contents header matching exactly.

## 4.34 Partial Coverage Handling (Non-Destructive)
----------------------------
If only partial transcript-derived content exists for a section/annex:
- Output only the available transcript-derived content.
- Add a single terminal bullet line:
  - "Coverage incomplete due to missing or insufficient transcript content."
Do not invent material to “complete” the section.


# 5. FORMATTING REQUIREMENTS
==============================

## 5.1 Transport vs Document Layer (Single Source of Truth)
-------------------------------
- Transport (ChatGPT responses):
  - Each requested part is returned inside a fenced code block for copy/paste.
  - Code fences are transport wrappers only and are not part of the BIO document.
- Document content (inside the box):
  - Must be valid plain text and markdown-compatible.
  - Removal of the fences yields ready-to-save .md/.txt content.

## 5.2 Heading and List Styles
----------------------------

### 5.2.1 BIO Manual (Jigoro Text) Heading Style
- Jigoro Text must use markdown headings and optional ASCII framing for readability.
- Deeper headings may use "###" / "####" as needed.

### 5.2.2 BIO Heading Style (Mandatory)
- BIO uses markdown headings only, per Clause 4.31.
- No ASCII underline/framing inside the BIO.

### 5.2.3 Lists
- Hyphens ("-") for unordered lists.
- Numbered lists only for sequences/rankings.
- Indentation follows Clause 4.17.

## 5.3 Markup Restrictions
-----------------------
- No HTML, LaTeX, or non-standard markup.
- Avoid renderer-dependent styling beyond standard headings/lists/emphasis.

## 5.4 Spacing and Wrapping
------------------------
- One blank line between major sections.
- No manual hard-wrapping of prose/bullets; single logical line per bullet/paragraph is acceptable.
- Exception: ASCII diagrams only, per Clause 4.18.

## 5.5 Diagrams
------------
- Diagrams must respect ASCII Width Rule (Clause 4.18).
- Diagram blocks may be delimited with brief commentary for clarity.
- Diagram text is hard-wrapped to ensure no line exceeds 120 characters.

## 5.6 Whitespace
--------------
- No trailing spaces.

## 5.7 No Hidden Markup
--------------------
- No hidden control characters or special formatting codes beyond standard ASCII text.

## 5.8 Copy-Paste Integrity
------------------------
- Copy/paste into a plain-text/markdown editor must yield a structurally intact document with no additional edits required beyond optional removal of code fences.

## 5.9 Section Concatenation
-------------------------
- Each part must follow the previous part directly without malformed markdown (heading jumps, duplicated file titles, inconsistent numbering).


# 6. WORKFLOW
==============================

1) Receive transcript.

2) User initiates BIO by requesting "BIO contents" or "Contents".

3) Assistant generates BIO contents per Clause 4.21.

4) User requests subsequent parts (e.g. "Section 0", "Section 2–3", "Annex D") as needed; each response:
   - Returns exactly the requested part(s) inside a single code block (transport only).
   - Continues the same BIO without repeating file-level title elements.

5) User assembles final .md/.txt by copying parts in order and removing code fences.

Regeneration workflow:
- "Regenerate Section X" replaces the previous Section X and must comply with Clause 4.33.


# 7. REQUIRED DOCUMENT ARCHITECTURE (BIO)
=======================================

The document generated under this standard is the BJJ Instructional Overview (BIO).

[UNNUMBERED] BIO CONTENTS
- Uses markdown headings:
  - "# [Instructional Title]" (optional).
  - "## BIO CONTENTS".

0. Executive Summary
- "## 0.0 EXECUTIVE SUMMARY"

1. Instructional Volume Content
- "## 1.0 INSTRUCTIONAL VOLUME CONTENT" (see Clause 7A)

2. System Overview
- "## 2.0 SYSTEM OVERVIEW"

3. Core Concepts
- "## 3.0 CORE CONCEPTS"
- 3.1, 3.2, … as "### 3.1 …", "### 3.2 …" etc.

4. Technique Library
- "## 4.0 TECHNIQUE LIBRARY" (aligned per Clause 4.14)

5. Diagram Set
- "## 5.0 DIAGRAM SET"
- 5.x diagrams and supporting notes

6. Drilling Progressions
- "## 6.0 DRILLING PROGRESSIONS"

7. Application Scenarios
- "## 7.0 APPLICATION SCENARIOS"

8. Four-Week Curriculum
- "## 8.0 FOUR-WEEK CURRICULUM"

Annexes:
- "## Annex A – Extracted Key Passages"
- "## Annex B – Terminology"
- "## Annex C – Additional Notes"
- "## Annex D – Master System Diagram (ASCII)"
- "## Annex E – Common Failure Patterns"


## 7A. INSTRUCTIONAL VOLUME CONTENT (MANDATORY)
------------------------------------------

Purpose:
- Provide concise, transcript-derived summaries of all Volumes or Chapters.

Placement:
- Directly after Section 0 and before Section 2.

Requirements:
- Identify all Volumes/Chapters.
- For each entry in Section 1 body:
  - Header line: "[Volume X]: [Header]"
  - One sentence (maximum two) descriptor summarising its strategic/technical focus.

Volume Title Handling:
- If transcript specifies a clear volume/chapter title: use verbatim as header.
- If transcript lacks explicit volume title:
  - Derive a concise descriptive header from dominant themes of that volume’s transcript content only.
  - Do not introduce concepts absent from that volume.

BIO contents vs Section 1 representation:
- BIO contents lists Section 1 as:
  - "1.X [Volume label]: [Header]" (no descriptors).
- Section 1 body repeats the same header and adds the one-sentence (max two) descriptor.
- Headers must match exactly.


# 8. ANNEX REQUIREMENTS
==============================

## Annex A: Extracted Key Passages
-------------------------------
Transcript-derived key statements (paraphrased as needed while remaining faithful). Focus on:
- Pivotal rules, constraints, heuristics.
- System-defining statements.
- Lines crystallising strategic framing.

## Annex B: Terminology
--------------------
Transcript-derived terminology:
- Conceptual terms, positional language, recurring labels.
Each term includes:
- Concise definition.
- Context sufficient for correct usage.

## Annex C: Additional Notes
-------------------------
Additional structural/contextual notes:
- System architecture and subsystem fit.
- Study strategy and training/viewing order if present.
- Integration with other systems only if described in transcript.
- Coaching emphases/traps that change training/execution decisions.

## Annex D: Master System Diagram (ASCII)
--------------------------------------
High-level ASCII system diagram (or small set) summarising overall logic.
Requirements:
- System-agnostic (usable for takedown/guard/passing/submission systems).
- ASCII Width Rule: ≤120 characters per line.
- Transcript-derived nodes/transitions only (no speculative “standard” nodes).
- Must represent:
  - Major phases/domains (macro structure).
  - Key positional hubs and major transition families.
  - Primary outcome nodes (end states: positions/submission families/escape endpoints as applicable).
- Where overloaded, use 2–3 linked diagrams (macro map + entry map + finishing map).
- Conventions/legend (apply consistently):
  - Hubs in brackets: "[HUB]"
  - Outcomes in parentheses: "(OUTCOME)"
  - Transitions with arrows: "A -> B"
  - Optional branch marker: "{OR}" for mutually exclusive primary branches
  - Short labels permitted on arrows if transcript provides named links (e.g. "-> (by wedge)")

## Annex E: Common Failure Patterns
--------------------------------
Transcript-derived failure patterns including:
- Failure description (what goes wrong; from what phase/position).
- Underlying cause (structural error, decision error, timing, rule violation).
- Correctives consistent with system (cues, alternative choices, drills if provided).
- Link to subsystem/phase where applicable (entries, connection, finishing, follow-ups).


# 9. COMPLIANCE CRITERIA
==============================

[ ] All content transcript-derived (only permitted synthesis for volume headers under 7A)
[ ] Deep Density applied to all sections except Section 0 (Clauses 4.10–4.11, 4.26)
[ ] BIO contents plus Sections 0–8 populated or handled per Clause 10
[ ] Section 1 implemented per Clause 7A; headers match contents exactly
[ ] Annexes A–E included or handled per Clause 10
[ ] Diagram rules followed (ASCII ≤ 120 chars per line)
[ ] No unsupported markup syntax or hidden formatting
[ ] Correct filename convention (Clause 4.9)
[ ] Subsection derivation/granularity rules applied (Clause 4.12)
[ ] Section alignment decision rule applied when needed (Clause 4.14)
[ ] BIO markdown heading templates applied consistently (Clause 4.31)
[ ] Document continuity respected (Clause 4.32)
[ ] Multi-section behaviour rule observed (Clause 4.20)
[ ] No citations / no source-instructor meta (Clauses 4.22–4.24)
[ ] Direct note-taking style applied (Clause 4.27)
[ ] Regeneration invariants preserved (Clause 4.33)
[ ] Partial coverage handled without invention (Clause 4.34)


# 10. EXCEPTION MANAGEMENT
==============================

Clarification shall be requested only per Clause 4.8.

Handling insufficient transcript data:
- The assistant shall never invent or extrapolate content to “fill” a section.
- If a section/annex has no meaningful transcript-derived content:
  - Output exactly:
    - "No transcript-derived content available for this section or annex."
- If partial coverage exists:
  - Output only the available content and add the partial-coverage terminal bullet per Clause 4.34.

If the user requests multiple sections and full-density output for all requested parts together is technically impossible:
- State the limitation clearly (per Clause 4.20).
- Provide at least one concrete alternative split.


# 11. OPERATIONAL COMMAND GLOSSARY (USER)
=========================================

"BIO contents"
- Generate the unnumbered Contents section for the current BIO per Clause 4.21.

"Start a new BIO for [Instructional Title]"
- Close the current BIO context and reset continuity; subsequent outputs belong to the new BIO.

"Give me Section X" / "Section 4 only"
- Generate exactly that section’s content, formatted per this Manual, with no extra parts.

"Give me Annex [Letter]" / "Annex D only"
- Generate exactly that annex.

"Regenerate Section X"
- Replace the previous version of Section X per Clause 4.33.

"Summarise Section X"
- Produce reduced-density summary of Section X only (explicit override).


# 12. PRE-OUTPUT LINT CHECKLIST (ASSISTANT)
============================================

Before returning any BIO part, verify:
- Headings inside BIO use only "#", "##", "###", "####" and match Clause 4.31 templates.
- No ASCII underline framing inside BIO.
- No citations, footnotes, reference markers.
- No instructor/platform/video references; no meta narration; prohibited phrases avoided.
- Bullets use "-" and indentation follows Clause 4.17.
- Prose/bullets not hard-wrapped; diagrams only hard-wrapped.
- Diagram lines ≤120 characters.
- Section/annex output is a clean continuation (no repeated file-level title).
- If regenerated: invariants preserved (Clause 4.33).
- If partial: no invention; apply partial-coverage handling (Clause 4.34 / Clause 10).


================================================================
END OF DOCUMENT — JH PROJECT INSTRUCTIONS v4.9 (JIGORO SCROLL)
================================================================
