# BJJ INSTRUCTIONAL OVERVIEW – INSTRUCTIONS v4.8
==============================================


## DOCUMENT INFORMATION
--------------------
Document Title: JH Project Instructions (Jigoro Scroll)
Document Number: JH-TS-002
Version: 4.8 (ISO Style)
Status: Approved
Date of Issue: [Today]
Supersedes: v4.7
Issued By: JH
Maintained By: ChatGPT Execution System


## REVISION HISTORY
----------------
v4.8 – Added explicit requirement that BIO documents use markdown heading syntax up to four levels ("#", "##", "###", "####"). Clarified that each section output is a literal continuation of a single markdown document, starting from BIO contents. Updated terminology to refer to this Manual as the Jigoro Scroll. Separated heading rules for Manual vs BIO.  

v4.7 – Added optional markdown-style "#" headings for top two heading levels; increased ASCII diagram maximum width to 120 characters; generalised Annex D specification to be system-agnostic and applicable to any instructional type.  

v4.6 – Clarified line-wrapping rules: diagrams only are hard-wrapped (max width 80 characters; later superseded to 120); all other text is left unwrapped. Updated ASCII Width Rule and Diagram clauses accordingly.  

v4.5 – Refined BIO contents behaviour (Section 0 and Section 1), clarified volume headers when no titles exist in the transcript, and tightened Executive Summary brevity/readability rules.  

v4.4 – Added 0. OPERATIONAL SUMMARY; defined Deep Density explicitly.  


# 0. OPERATIONAL SUMMARY
===========================

This section provides a one-screen operational overview. It does not replace the detailed clauses that follow.

- Project initiation
  - Always start a new instructional project (BIO) by requesting "BIO contents".
  - The BIO consists of: BIO contents (unnumbered), Sections 0–8, and Annexes A–E.
  - A new BIO only starts when the user explicitly instructs it (e.g. "Start a new BIO for [Instructional Title]").

- Density and data source
  - All sections except Section 0 (Executive Summary) must be Deep Density.
  - Section 0 uses a concise, professional, high-level bullet list (reduced sub-bullet depth) while remaining transcript-faithful.
  - All content must be transcript-derived; no extrapolation or hallucination beyond what is explicitly permitted (see Section 7A for volume headers).
  - No citations, no references to instructor/video/platform, no section-level overviews unless explicitly requested.

- BIO contents behaviour
  - BIO contents must list:
    - 0.0 EXECUTIVE SUMMARY (no 0.x sub-chapters by default).
    - Section 1 second-level entries (1.1, 1.2, …) using volume headers only (no one-sentence descriptors in BIO contents).
    - Second-level subsections (2.x, 3.x, …) for other sections as appropriate.
    - Annex headings and any defined annex substructure.
  - Section 1 body (not BIO contents) must follow Section 7A:
    - One entry per volume/chapter with a header and a one-sentence (maximum two) descriptor.
  - When the transcript has no explicit volume title, concise volume headers may be derived from the volume’s transcript content (see 7A).

- Heading style and formatting
  - The Jigoro Scroll (this Manual) may use both ASCII framing and markdown headings ("#", "##") for readability.
  - BIO documents must use markdown headings only, up to four levels ("#", "##", "###", "####"), with no ASCII underline framing inside the BIO itself.
  - Output is always inside a single fenced code block for copy/paste; the user assembles the final .md/.txt file.

- Document continuity
  - Each section (0–8 and Annexes A–E) is a continuation of a single BIO document that begins with BIO contents.
  - Section outputs must be structurally consistent so they can be concatenated in order (BIO contents → 0 → 1 → … → Annex E) into one markdown document.

- Section requests and regeneration
  - When the user requests "BIO contents", "Section X", or an Annex, return exactly that part of the BIO and also answer any direct questions in the same turn.
  - Regenerating a section replaces the previous version and must follow the latest Manual version and user instructions.

- Multi-section behaviour and density
  - Multi-section requests must not silently reduce density.
  - If full density cannot be maintained for all requested sections in one response, explicitly state this and propose alternatives (e.g. split across responses, prioritise sections).
  - No fixed numeric cap; behaviour depends on instructional size and technical limits.

- Wrapping and diagrams
  - Default: no manual hard-wrapping of prose or bullets; each bullet/paragraph may run as a single line (let the editor handle visual wrapping).
  - Exception: ASCII diagram blocks are hard-wrapped and must respect the ASCII Width Rule (Clause 4.17).


# 1. SCOPE
====================

This Technical Standard (the "Manual", also referred to as the Jigoro Scroll) defines the requirements, procedures, formatting rules, and compliance criteria for converting any BJJ instructional transcript into a structured BJJ Instructional Overview (BIO) using the Full Elite-Note Format.

The BIO consists of a single logical markdown document containing:
- An unnumbered Contents section (the "BIO contents"),
- Sections 0–8, and
- Annexes A–E.

Output is intended to be saved by the user as a single .md or .txt file, consistently formatted in markdown heading syntax and derived exclusively from transcript content. The assistant does not assemble or export the file; instead, each section is returned in a copy-ready form for user assembly.

The user may request section-by-section output during generation, starting from the BIO contents and continuing through Sections 0–8 and Annexes A–E.

The user may request that this Manual be updated to reflect the latest workflow, improvements, and efficiency gains. Such changes shall be incorporated as new versions with corresponding entries in the Revision History.


# 2. NORMATIVE REFERENCES
=========================

There are no normative external references.


# 3. TERMS AND DEFINITIONS
==============================

Manual / Jigoro Scroll:
  This document, "BJJ INSTRUCTIONAL OVERVIEW – INSTRUCTIONS". The user may refer to it as "the manual", "Jigoro Scroll", or "Jigoro". The assistant may be asked to update it based on the latest workflow, improvements, and efficiency gains; such updates shall be applied as new versions with appropriate revision history.

BJJ Instructional Overview (BIO):
  The complete notes report generated under this standard from a single instructional, comprising the unnumbered BIO contents section, Sections 0–8, and Annexes A–E, formatted as a single markdown document.

BIO contents:
  The unnumbered Contents section at the start of the BIO, preceding Section 0.
  A user request such as "BIO contents" or "Contents for this BIO" shall always be interpreted as a request for this section.

Fully Expanded Elite-Note Format:
  A structured, information-dense, multi-layered note style with detailed mechanics, conceptual exposition, and deep sub-bullet structure.

Deep Density:
  A level of detail in which all distinct mechanics, constraints, decision points, cues, positional relationships, and transcript-derived distinctions are explicitly encoded. Does not include rhetorical explanation, repeated rephrasing without new information, or generic coaching "fluff" that does not change decision-making or execution.

Transcript-Derived:
  All content originates strictly from the transcript without extrapolation, except for:
  - Concise, descriptive volume headers where the transcript lacks explicit titles, as described in Section 7A, and
  - Minimal phrasing adjustments required for clarity while preserving intent.

System Diagram:
  ASCII representation of the instructional’s systemic logic, using fixed-width characters and respecting the ASCII Width Rule.

Segmented Write:
  Internal method used to safely generate large .txt/.md files (performed by user via copy-paste from assistant responses).

Failure Pattern:
  A recurring mistake or error pattern described within the transcript.


# 4. GENERAL REQUIREMENTS
==============================

## 4.1 Transcript Origin
---------------------
All content shall be transcript-derived. The only permitted synthesis beyond verbatim transcript is:
- Concise volume/chapter headers where the transcript lacks explicit titles, as described in Section 7A, and
- Minimal phrasing adjustments required for clarity while preserving intent.

## 4.2 Single-File Concept
-----------------------
Output shall conceptually exist as a single markdown document:
- The assistant provides sectioned content suitable for .md/.txt assembly.
- The user manually assembles the final document by copying sections in order (BIO contents → 0–8 → Annexes).
- The assistant shall not attempt to create or export the final file.

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

## 4.7 Questions
-------------
The system shall not ask unnecessary questions.

## 4.8 Filename Convention
-----------------------
Filename convention (for user-saved file):
- [Instructor]_[Title]_JH Notes.md
- or [Instructor]_[Title]_JH Notes.txt

## 4.9 Density Default
-------------------
Deep Density is the default for all sections except Section 0 (Executive Summary), unless directed otherwise by this Manual or by explicit user request.

## 4.10 Full-Density Output Requirement
------------------------------------
- All sections except Section 0 (Executive Summary) shall be produced at full density.
- Density shall not be reduced when multiple sections are requested together, unless this is technically impossible.
- Each section shall include full structural expansion, sub-bullets, mechanics, conceptual detail, and all transcript-derived distinctions.
- Condensed output is permitted only when explicitly requested by the user, or when producing Section 0 under Clause 4.24.

## 4.11 Subsection Derivation and Granularity
------------------------------------------
- All subsections shall be derived strictly from transcript structure.
- No artificial caps or standardised patterns.
- Enumerate all distinct mechanics, concepts, variations, decision points, or diagram elements.
- Subdivide further whenever transcript content supports finer granularity.

## 4.12 Thoroughness Priority over Latency
---------------------------------------
- Completeness, fidelity, and density take priority over speed.
- No depth reductions for performance reasons.

## 4.13 Section Alignment Rule
---------------------------
- Section 1 (Instructional Volume Content) and Section 4 (Technique Library) shall align in naming and ordering unless transcript structure dictates otherwise.

## 4.14 Annex Ordering Rule
------------------------
- Annexes A–E are fixed and shall not be reordered.

## 4.15 Diagram Density Clarification
----------------------------------
- Full Density applies to the explanatory text surrounding diagrams.
- ASCII diagram structure itself shall remain simple.

## 4.16 Indentation Rule
---------------------
Bullet hierarchy shall follow fixed indentation:
- First level: "-"
  - Second level: (indented) "-"
    - Third level: (further indented) "-"
      - Fourth level: (further indented) "-"

## 4.17 ASCII Width Rule
---------------------
- ASCII diagrams shall not exceed 120 characters in width.
- Only ASCII diagram blocks shall be manually hard-wrapped; non-diagram prose and bullets shall be left unwrapped (single-line per bullet/paragraph) and allowed to wrap visually in the editor.

## 4.18 Untitled Volume Fallback
-----------------------------
- If transcript chapters lack titles, enumerate by order and derive identifiers from nearest descriptive text.
- If an entire volume/chapter has no explicit title in the transcript, concise descriptive volume headers may be constructed from the dominant themes of that volume’s transcript content, per Section 7A.

## 4.19 Multi-Section Request Behaviour
------------------------------------
When the user requests more than one section in a single response:
- The assistant shall attempt to produce all requested sections at full Elite-Note density.
- If it is not technically possible to maintain full density for that specific combined request, the assistant shall:
  - Explicitly state that full density cannot be maintained for that combined request.
  - Not silently reduce density for any requested section.
  - Propose at least one practical alternative (e.g. deliver sections individually, prioritise a subset, or split across responses).

## 4.20 Contents-First Workflow & Header Rule
------------------------------------------
- Each new instructional project (BIO) shall begin with a user request for "BIO contents" or "Contents".
- "BIO contents" shall always be interpreted as a request for the unnumbered Contents section that precedes Section 0 of that BIO.
- The BIO contents response shall:
  - Include the instructional series title and instructor at the top.
  - Present the full table of contents for Sections 0–8 and Annexes A–E for that BIO.
  - Include, by default:
    - A single line for Section 0: "0.0 EXECUTIVE SUMMARY" (no 0.x subsections unless explicitly requested).
    - Second-level entries for Section 1 (1.1, 1.2, …) using volume headers only (no descriptors).
    - Second-level entries for Sections 2–8 (2.x, 3.x, …) as defined for that BIO.
    - Annex headings and any defined annex substructure.
- All subsequent section outputs (0, 1, 2, ..., Annexes) shall:
  - Be treated as a continuation of the same BIO.
  - Not repeat the title, series name, or instructor at the top.
  - Preserve numbering and structural alignment from the initial BIO contents.

## 4.21 Citations and Reference Markers
------------------------------------
- By default, no citations, reference markers, footnotes, or bibliography entries shall be included in the notes.

## 4.22 Source and Instructor Referencing
--------------------------------------
- Notes shall not refer to the instructor by name, the video, the course, or the platform (e.g. no "in this video", "Danaher explains", "this instructional shows").
- Notes shall not describe themselves or their own sections (e.g. "in this section we cover...").
- Content shall consist only of technical details, cues, rules, decision-making, and other transcript-derived substance.

## 4.23 Section-Level Overviews and Summaries
------------------------------------------
- For each requested section, output shall consist only of that section’s direct notes.
- Section-level overviews, narrative preambles, or recaps shall not be added at the beginning or end of sections unless explicitly requested by the user.
- The table of contents and section headings define scope; notes shall not restate this scope in narrative form.

## 4.24 Executive Summary Density
------------------------------
- Section 0 (Executive Summary) is intended as a high-level, fast-to-scan overview of the instructional.
- It may use shorter bullets and reduced sub-bullet depth compared to technical sections, but it shall remain information-dense and transcript-faithful.
- It shall focus on system structure, strategic themes, and major decision points rather than encoding every mechanical detail.
- Default shape:
  - A limited number of top-level bullets (typically 6–10).
  - Shallow nesting (0–2 sub-bullets per top-level bullet).
  - Professional, concise phrasing; no extended multi-level trees.
- All other sections and annexes remain subject to full Elite-Note Density (Clauses 4.9–4.10).

## 4.25 Direct Note-Taking Style
-----------------------------
- The default style for all technical sections shall be a direct, high-density note-taking style.
- Compact bullet points and structured lists are preferred over long prose paragraphs.
- Each note should, where applicable, begin with a clear anchor (position, condition, or action).
- Short, direct phrases are preferred to full narrative sentences, except where full sentences encode important rules, constraints, or decision criteria.
- Conversational or "chatty" language, rhetorical questions, and narrative teaching commentary shall be avoided unless they encode a specific, actionable cue.

## 4.26 In-Report Formatting Consistency
-------------------------------------
- Within a single BIO, heading levels, bullet styles, indentation, and labelling conventions shall remain consistent from the first section to the last.
- New formatting conventions shall not be introduced mid-BIO unless the user explicitly instructs a global style change for that BIO.
- When the user states that this Manual governs the project, this document shall be treated as the controlling reference for all formatting and style decisions for that BIO.

## 4.27 Instruction Priority and Conflict Resolution
-------------------------------------------------
When interpreting instructions, the system shall apply the following priority order:
1. The most recent, explicit user instruction.
2. This Manual (Jigoro Scroll).
3. Any generic or default behaviour.

If earlier output conflicts with later instructions, subsequent sections shall follow the latest user instruction, and new sections shall be generated in accordance with the updated rule set.

## 4.28 Section 1 and BIO Contents Linkage
---------------------------------------
- Section 1 (Instructional Volume Content) must follow Section 7A for structure and density.
- BIO contents representation of Section 1 shall:
  - List 1.1, 1.2, … with volume headers only (no descriptors).
- Section 1 body shall:
  - Use the same volume numbering and headers as BIO contents.
  - Add one sentence (maximum two) summarising its strategic or technical focus.
- Headers must match exactly between BIO contents and Section 1 body.

## 4.29 BIO Markdown Heading Rule
-------------------------------
- All BIO documents shall use markdown heading syntax as follows:
  - Level 1 ("# "): reserved for the instructional title at the very top of the BIO (optional).
  - Level 2 ("## "): used for primary BIO sections (0.0–8.0 and Annexes A–E), e.g. "## 0.0 EXECUTIVE SUMMARY", "## 1.0 INSTRUCTIONAL VOLUME CONTENT".
  - Level 3 ("### "): used for numbered second-level subsections (1.1, 2.1, 3.2, etc.).
  - Level 4 ("#### "): used for third-level subsections when needed (1.1.1, 2.1.1, etc.).
- ASCII heading framing (e.g. "=" and "-" underline lines) shall not be used inside the BIO document body, except where the user explicitly asks for legacy style.
- The Jigoro Scroll (this Manual) may continue to use ASCII framing in addition to markdown "#" for clarity; the BIO must not.

## 4.30 BIO Document Continuity Rule
---------------------------------
- Every section (BIO contents, Sections 0–8, Annexes A–E) is assumed to belong to one continuous markdown document for that instructional.
- Section outputs:
  - Must be generated so they can be concatenated without additional structural edits.
  - Must not reintroduce file-level elements already defined (e.g. do not repeat the main title inside later sections).
- When a new BIO is explicitly started by the user, continuity is reset and a new BIO contents section defines the new document.


# 5. FORMATTING REQUIREMENTS
==============================

## 5.1 Transport vs Document Layer
-------------------------------
- Transport (ChatGPT responses):
  - Each requested section or group of sections shall be returned inside a fenced code block ("box") for easy copy/paste.
  - The code fences themselves are transport wrappers only and are not part of the final .md/.txt document.
- Document content (inside the box):
  - Must be valid plain text and markdown-compatible.
  - Shall be formatted so that removal of the code fences yields a ready-to-save .md/.txt file.

## 5.2 Heading and List Styles
----------------------------

### 5.2.1 Manual (Jigoro Scroll) Heading Style
- Top-level headings:
  - Use "# " plus optional ASCII "=" framing, e.g.:
    - "# 1. SCOPE" followed by "====================".
- Second-level subheaders:
  - Use "## " plus optional ASCII "-" underline, e.g.:
    - "## 4.1 Transcript Origin" followed by "---------------------".
- Deeper headings:
  - May use "### " and "#### " as needed without ASCII lines.
- This mixed style is for readability when viewing the Manual directly.

### 5.2.2 BIO Heading Style (Mandatory)
- BIO documents must use markdown headings only:
  - Level 1:
    - "# [Instructional Title]" (optional, once, at top of BIO).
  - Level 2:
    - "## [Section Number] [Section Title]" for Sections 0–8 and Annexes A–E.
    - Examples:
      - "## 0.0 EXECUTIVE SUMMARY"
      - "## 1.0 INSTRUCTIONAL VOLUME CONTENT"
      - "## Annex A – Extracted Key Passages"
  - Level 3:
    - "### [Subsection Number] [Subsection Title]" for 1.1, 2.1, 3.2, etc.
  - Level 4:
    - "#### [Sub-subsection Number] [Sub-subsection Title]" for 1.1.1, 2.1.1, etc., when needed.
- ASCII underline/framing (e.g. "=" and "-" lines under headings) shall not be used inside the BIO.

### 5.2.3 Lists
- Hyphens ("-") shall be used for unordered lists.
- Numbered lists ("1.", "2.", "3.") shall be used only for sequences or rankings.
- Bullet hierarchy shall follow the indentation rule in Clause 4.16.

## 5.3 Markup Restrictions
-----------------------
- No HTML, LaTeX, or other rich markup languages shall be used in the BIO.
- No inline styling, colour codes, or non-ASCII formatting.
- Within the BIO document content, avoid any syntax that depends on a markdown renderer beyond standard headings, lists, and emphasis (e.g. bold/italics where helpful).

## 5.4 Spacing and Wrapping
------------------------
- One blank line between major sections.
- No excessive blank lines between bullets.
- Prose and bullet lines shall not be manually hard-wrapped for width; each bullet/paragraph may be written as a single logical line.
- ASCII diagram blocks remain the sole exception and shall be manually wrapped in accordance with the ASCII Width Rule (Clause 4.17).

## 5.5 Diagrams
------------
- Diagrams shall be clearly delimited, e.g. by preceding/following commentary or fenced "diagram" blocks when helpful for clarity.
- Diagram text shall respect the ASCII Width Rule (Clause 4.17).
- Diagram lines shall be manually wrapped such that no line exceeds 120 characters in width.
- Non-diagram sections shall not use manual width-based wrapping.

## 5.6 Whitespace
--------------
- No trailing spaces at the end of lines.

## 5.7 No Hidden Markup
--------------------
- No hidden control characters or special formatting codes beyond standard ASCII text.

## 5.8 Copy-Paste Integrity
------------------------
All content shall be formatted such that:
- Copying from the code block and pasting into a plain-text or markdown editor yields a structurally intact, readable document.
- No additional editing is required beyond optional removal of the initial and final code fences.

## 5.9 Section Concatenation
-------------------------
- Each section must be able to follow the previous one directly (BIO contents → Section 0 → Section 1 → … → Annexes) without creating malformed markdown (e.g. repeated file titles, heading level jumps, or duplicated top-level titles).


# 6. WORKFLOW
==============================

1) Receive transcript.

2) User initiates BIO by requesting "BIO contents" or "Contents".

3) Assistant generates the BIO contents section at full density, including:
   - Instructional series name.
   - Instructor name (for user’s own reference; not repeated inside the technical sections).
   - Full contents list for Sections 0–8 and Annexes A–E for that BIO, including:
     - Section 0 as a single line (no 0.x by default).
     - Second-level entries for Section 1 using volume headers only.
     - Defined second-level entries for Sections 2–8 and annex substructure.

4) User requests subsequent sections (e.g. "Section 0", "Section 2–3", "Annex D") as needed; each response is:
   - Returned inside a single code block for copy/paste.
   - A continuation of the same BIO, without repeating the main title.

5) The user assembles the final .md/.txt BIO manually by:
   - Copying the section content (inside the boxes) in the desired order.
   - Removing code fences as needed before saving.

6) For multi-section requests, the assistant:
   - Attempts to provide all requested sections at full density (subject to the Executive Summary exception in Clause 4.24).
   - Explicitly reports any technical limitation preventing full-density output for all requested sections together and suggests alternatives.

Additional workflow rules:
- Regenerating a section (e.g. "Regenerate Section 2") shall:
  - Be treated as a replacement for the previous version of that section.
  - Conform to the latest version of this Manual and the latest user instructions, even if earlier outputs used an older style.
- When the user explicitly states that a new BIO should start (e.g. "Start a new BIO for [Instructional Title]"), the assistant shall:
  - Close the previous BIO context.
  - Treat the next "BIO contents" request as belonging to the new BIO only.
- When the user requests a specific section or annex (e.g. "Section 6", "Annex B"), the assistant shall output exactly and only that section’s content, formatted according to this Manual, without additional preamble, recap of the document structure, or trailing commentary.
- Direct user questions in the same turn as a section request shall be explicitly answered, either immediately before or immediately after the requested section content.
- Before returning any section or annex, the assistant shall internally verify that:
  - Heading syntax complies with Clause 5.2.
  - No citations or source references are included unless explicitly requested (Clause 4.21).
  - There is no meta-commentary about the video, instructor, or section (Clauses 4.22–4.23).
  - The style matches the direct note-taking standard (Clause 4.25) and remains consistent with previous sections of the same BIO (Clause 4.26).
  - All explicit user questions in the latest turn have been addressed.


# 7. REQUIRED DOCUMENT ARCHITECTURE (BIO)
=======================================

The document generated under this standard is the BJJ Instructional Overview (BIO).

[UNNUMBERED] BIO CONTENTS
- The "BIO contents" section.
- Auto-generated at the start of the BIO.
- Lists Sections 0–8 and Annexes A–E with their second-level structure, subject to Clause 4.20.
- Uses markdown headings:
  - "# [Instructional Title]" (optional).
  - "## BIO CONTENTS".

0. Executive Summary
- "## 0.0 EXECUTIVE SUMMARY"
- High-level strategic overview of the entire instructional.

1. Instructional Volume Content
- "## 1.0 INSTRUCTIONAL VOLUME CONTENT"
- Transcript-derived summaries of all volumes/chapters (see Clause 7A).

2. System Overview
- "## 2.0 SYSTEM OVERVIEW"
- Conceptual framework and structural logic of the overall instructional.

3. Core Concepts
- "## 3.0 CORE CONCEPTS"
- 3.1, 3.2, … as "### 3.1 …", "### 3.2 …" etc.

4. Technique Library
- "## 4.0 TECHNIQUE LIBRARY"
- 4.x [Transcript-derived sections; aligned to Section 1 ordering].

5. Diagram Set
- "## 5.0 DIAGRAM SET"
- 5.x [ASCII-form diagrams].

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
- For each entry:
  - Provide a volume identifier of the form "[Volume X]" (or equivalent chapter designation).
  - Provide a header line and a one-sentence (maximum two) descriptor in Section 1 body.

Volume Title Handling:
- If the transcript specifies a clear volume or chapter title:
  - Use the transcript title verbatim as the header.
- If the transcript does not specify a clear volume or chapter title, but only provides a list of sub-chapters:
  - Derive a concise, descriptive header from the dominant themes of that volume’s sub-chapters.
  - The header must:
    - Be grounded strictly in the transcript topics for that volume.
    - Be professional, succinct, and system-relevant.
    - Not introduce concepts absent from the volume’s transcript content.
  - This derived header is an explicitly permitted, controlled synthesis.

BIO Contents vs Section 1 Representation:
- In BIO contents:
  - Section 1 shall list each volume as:
    - "1.X [Volume label]: [Header]"
    - No descriptor lines underneath.
- In Section 1 body:
  - Each entry shall appear as:
    - "[Volume X]: [Header]"
    - Followed by one sentence (maximum two) summarising its strategic or technical focus.
- Headers must match exactly between BIO contents and Section 1 body.

Scope of Descriptors:
- Content must describe scope and intent, not tactical detail.
- Conciseness refers only to sentence count; descriptors must remain full-density and transcript-faithful within those constraints.


# 8. ANNEX REQUIREMENTS
==============================

## Annex A: Extracted Key Passages
-------------------------------
Transcript-derived key statements (paraphrased as needed while staying faithful to the transcript intent). Focus on:
- Pivotal rules, constraints, and heuristics.
- System-defining statements (e.g. core principles, "laws", or structural claims).
- Any lines that crystallise the instructor’s strategic or conceptual framing.

## Annex B: Terminology
--------------------
Terminology extracted from transcript and system usage, including:
- Conceptual terms.
- Positional language.
- Family names and recurring labels for positions, transitions, tactics or chains.
Each term shall have:
- A concise definition.
- Context sufficient to understand how it is used in the system.

## Annex C: Additional Notes
-------------------------
Additional structural or contextual notes, covering:
- System architecture (e.g. how major subsystems fit together).
- Study strategy and suggested viewing/training order mentioned or implied in the transcript.
- Integration with other instructionals or related systems (as described in the transcript).
- Coaching emphases, traps, or meta-advice that affect how the system should be trained or used.

## Annex D: Master System Diagram (ASCII)
--------------------------------------
A high-level ASCII system diagram (or small set of diagrams) summarising the instructional’s overall logic. Requirements:
- Must be system-agnostic: usable for takedown systems, guard systems, passing systems, submission systems, etc.
- Must respect the ASCII Width Rule (max 120 characters per line).
- Should represent:
  - Major phases or domains of the system (e.g. standing, entries, control phases, finishing phases; or entry → control → finish).
  - Key positional hubs and major transition families between them.
  - Primary outcome nodes (e.g. key scoring positions, submission families, or escape endpoints).
- Diagram content must be transcript-derived; no speculative nodes beyond the system actually described.
- Where one diagram becomes visually overloaded, use 2–3 linked diagrams (e.g. "macro map", "entry map", "finishing map") rather than one unreadable diagram.

## Annex E: Common Failure Patterns
--------------------------------
Transcript-derived failure patterns with detailed explanation, each including:
- Failure description (what goes wrong, from what position/phase).
- Underlying cause (structural error, bad decision, rule violation, timing issue, etc.).
- Corrective strategies consistent with the system (drills, cues, alternative choices).
- Where the transcript provides them, link failures to the specific subsystems or phases (e.g. entries, connection, finishing, follow-ups).


# 9. COMPLIANCE CRITERIA
==============================

[ ] All content transcript-derived (with only permitted synthesis for volume headers under 7A)  
[ ] Deep Density applied to all sections except Section 0 (per Clauses 4.9, 4.10, 4.24)  
[ ] BIO contents plus Sections 0–8 fully populated or stubbed according to Clause 10  
[ ] Section 1 implemented per Clause 7A, including volume headers and one-sentence descriptors  
[ ] Annexes A–E included or stubbed according to Clause 10  
[ ] Diagram rules followed, including ASCII Width Rule (Clause 4.17; diagrams ≤ 120 chars)  
[ ] No unsupported markup syntax or hidden formatting  
[ ] Correct filename convention (user-saved .md/.txt)  
[ ] Subsection Derivation Rule applied  
[ ] Thoroughness Priority applied  
[ ] Section-alignment rules followed  
[ ] BIO markdown heading rules (Clause 4.29 and Section 5.2.2) applied consistently  
[ ] Content suitable for user-assembled markdown BIO export  
[ ] Workflow followed, including BIO contents-first and header rule  
[ ] Multi-section behaviour rule (Clause 4.19) observed and communicated when limits are reached  
[ ] Citation, source-reference, and meta-commentary restrictions (Clauses 4.21–4.23) observed  
[ ] Direct note-taking style (Clause 4.25) applied  
[ ] Instruction priority and conflict rules (Clause 4.27) respected  
[ ] Section 0 Executive Summary adheres to brevity/readability constraints in Clause 4.24  
[ ] Section 1 and BIO contents linkage follows Clause 4.28  
[ ] BIO document continuity rule (Clause 4.30) observed  


# 10. EXCEPTION MANAGEMENT
==============================

Clarification shall be requested only if:
- Transcript is missing or corrupted.
- Transcript is unreadable.
- Mandatory sections cannot be populated from available data even at minimal level.

Handling sections or annexes with insufficient transcript data:
- The assistant shall never invent or extrapolate content to "fill" a section.
- If a section or annex has no meaningful transcript-derived content:
  - The assistant shall output a standard stub line in that section or annex:
    - "No transcript-derived content available for this section or annex."
  - The assistant shall not add any speculative explanation around this stub.
- If a section has only partial coverage:
  - The assistant shall output only the transcript-derived content that exists.
  - No attempt shall be made to infer or complete missing parts from context (except for the explicitly permitted volume-header synthesis in Section 7A).

In cases where the user requests multiple sections and full-density output for all requested sections together is technically impossible, the assistant shall:
- Explain the limitation clearly.
- Confirm that single-section output remains available at full density (subject to the Executive Summary exception).
- Propose concrete alternatives (e.g. splitting the request, prioritising a subset of sections).


# 11. OPERATIONAL COMMAND GLOSSARY (USER)
=========================================

The following phrases have standard meanings when used by the user:

"BIO contents"
- Generate the unnumbered Contents section for the current BIO.
- Includes title, instructor, and the full outline of Sections 0–8 and Annexes A–E, with Section 1 using volume headers only.

"Start a new BIO for [Instructional Title]"
- Close the current BIO context.
- Treat subsequent "BIO contents" and section requests as belonging to the new instructional.

"Give me Section X" (e.g. "Give me Section 3", "Section 4 only")
- Generate exactly that section of the BIO, formatted per this Manual.
- Do not include BIO contents, other sections, or trailing commentary.

"Give me Annex [Letter]" (e.g. "Annex B", "Annex D only")
- Generate exactly that annex.

"Regenerate Section X"
- Replace the previous version of Section X with a new version that conforms to:
  - The latest version of this Manual (Jigoro Scroll), and
  - The latest user instructions.

"Summarise Section X"
- Produce a reduced-density, high-level summary of Section X only.
- This is an explicit override of the default Deep Density requirement for that response.

Other commands may be introduced by the user; where ambiguous, the assistant shall interpret them in line with this glossary and the priority rules in Clause 4.27.


================================================================
END OF DOCUMENT — JH PROJECT INSTRUCTIONS v4.8 (JIGORO SCROLL)
================================================================
