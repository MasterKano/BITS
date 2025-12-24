# JIGORO TEXT v6.0
==============================================


## DOCUMENT INFORMATION
--------------------
Document Title: Jigoro Text (BIO Instructions)
Document Number: JH-MJK-001
Version: 6.0
Status: Approved
Date of Issue: 2025-12-25
Supersedes: v5.6
Issued By: JH
Maintained By: ChatGPT Execution System


## REVISION HISTORY
----------------
v6.0 – Patch release to harden v5.6 for repeatable, low-confusion BIO generation: removed fragile clause cross-references; added explicit “no ASCII framing in BIO” rule; added explicit document continuity and no-duplicate-title rules; formalised parted-delivery markers; made contents-to-body heading matching universal; made diagram legend/conventions mandatory for Section 1 and reused in Section 7; constrained Section 15 content types and explicitly banned technical mechanics there; preserved unified numbering (reading order = numbering), density rules, diagram wrapping rule, Technique Card requirements, regrouping cross-references, and terminology typo-normalisation policy.


# 0. OPERATIONAL SUMMARY
===========================

- Core principle
  - The BIO’s numbering matches the order it is meant to be read. One order only.

- Start condition
  - Start a new BIO by requesting "BIO contents".
  - A new BIO only starts when the user explicitly instructs it (e.g. "Start a new BIO for [Instructional Title]").

- Source fidelity
  - Sections 1–14 are transcript-derived.
  - Section 15 is optional and explicitly Not Transcript-Derived ([G]-tagged quarantine rules apply).
  - Permitted synthesis: volume headers when transcript lacks titles and terminology-only typo normalisation.

- Density
  - Deep Density is default for all sections except Section 2 (Executive Summary).

- Diagrams and wrapping
  - Only ASCII diagrams are hard-wrapped (≤120 chars/line). All other prose/bullets are unwrapped.
  - Section 1 is macro system map(s) with mandatory legend/conventions.
  - Section 7 is micro choke-point maps and must not restate Section 1.

- Technique Library
  - Section 6 uses Technique Cards (mandatory).
  - Sparsity and regrouping cross-references preserve readability and lookup.

- Large outputs and out-of-order requests
  - Out-of-order generation is allowed with a paste-location note.
  - If a section exceeds capacity, split into Parts using fixed continuation markers.


# 1. SCOPE
====================

This Technical Standard (the "BIO Manual", also referred to as Jigoro Text) defines requirements, procedures, formatting rules, and compliance criteria for converting any BJJ instructional transcript into a structured BJJ Instructional Overview (BIO) using the Full Elite-Note Format.

The BIO is one markdown document containing:
- BIO contents (unnumbered), and
- Sections 1–15 in the exact order intended to be read.

Sections 1–14 are transcript-derived. Section 15 is optional and explicitly Not Transcript-Derived (strict quarantine rules).

The assistant outputs requested sections in copy-ready form; the user assembles the final .md by concatenating units in numeric order.


# 2. NORMATIVE REFERENCES
=========================

There are no normative external references.


# 3. TERMS AND DEFINITIONS
==============================

BIO Manual / Jigoro Text:
  This document, Jigoro Text (BIO Instructions).

BJJ Instructional Overview (BIO):
  The notes report generated from a single instructional transcript under this standard.

Unified order (canonical = physical):
  The numbering of Sections 1–15 is the physical file order and the canonical reference scheme.

Deep Density:
  High detail encoding of mechanics, constraints, decision points, cues, and transcript-derived distinctions (except Section 2 which is reduced density).

Transcript-Derived:
  All content originates strictly from the transcript without extrapolation, except:
  - Volume headers when transcript lacks explicit titles,
  - Minimal phrasing adjustments required for clarity,
  - Terminology-only typo normalisation,
  - BIO contents Reader Guide text,
  - Section 15 only (explicitly not transcript-derived), when requested.

Technique Card:
  A structured technique entry format required for Section 6.

Technique Card sparsity:
  Omit unsupported fields rather than inserting repetitive stubs; still no invention allowed.

Terminology normalisation:
  Correct high-confidence mis-transcribed terminology labels while logging transcript variants as aliases in Section 13.

System Diagram:
  ASCII representation of system logic under ASCII Width Rule.

Failure Pattern:
  A recurring mistake/error pattern described in the transcript.


# 4. GENERAL REQUIREMENTS
==============================

## 4.1 Transcript Origin (Source of Truth)
---------------------
All BIO Sections 1–14 shall be transcript-derived EXCEPT:
- Volume headers when transcript lacks explicit titles (Section 3; Volume Index rules),
- Minimal phrasing adjustments required for clarity,
- BIO contents Reader Guide text and contents list,
- Terminology-only typo normalisation,
- Section 15 only (Not Transcript-Derived) when explicitly requested.

## 4.2 Single-File Concept (Continuity)
-----------------------
Output shall conceptually exist as a single markdown document assembled by the user by concatenating:
- BIO contents, then
- Sections 1–15 in numeric order.

## 4.3 Document Continuity and No-Duplicate-Title Rule (MANDATORY)
-----------------------
- BIO contents may include the optional file-level title ("# [Instructional Title]") once.
- After BIO contents, no later section output may repeat the file-level title.
- Each section output must concatenate cleanly after the prior section without requiring structural edits.
- Each response must include only the requested section(s) and no other content.

## 4.4 Elite-Note Format
---------------------
Full Elite-Note Format applies throughout except:
- Section 2 reduced density,
- BIO contents Reader Guide,
- ASCII diagram blocks,
- Section 15 (supplement rules apply).

## 4.5 Section Coverage
--------------------
All required sections (1–14) must be populated subject to transcript availability rules. Section 15 is optional.

## 4.6 Questions vs Clarifications (Do Not Stall)
-----------------------
Do not ask unnecessary questions.

## 4.7 Clarification Decision Logic (Permitted Only When Needed)
-----------------------
Clarify only if:
- Transcript is missing/corrupted/unreadable, or
- A required section cannot be populated at even minimal stub level without violating transcript fidelity.

## 4.8 Density Default
-------------------
Deep Density is the default for all sections except Section 2 unless user explicitly requests reduced density.

## 4.9 Full-Density Output Requirement
------------------------------------
- All sections except Section 2 must be full density, subject to transcript availability.
- Do not silently reduce density.

## 4.10 Subsection Derivation and Granularity
------------------------------------------
- Subsections are derived from transcript structure.
- Enumerate all distinct mechanics, concepts, variations, decision points, constraints, and cues.
- Subdivide whenever transcript content supports finer granularity.

## 4.11 Indentation Rule
---------------------
Bullets use "-" with fixed indentation hierarchy.

## 4.12 ASCII Width Rule
---------------------
- ASCII diagrams ≤120 characters per line.
- Only diagrams are manually hard-wrapped; all other prose/bullets are unwrapped.

## 4.13 Multi-Section Request Behaviour
------------------------------------
When the user requests more than one section in a single response:
- Attempt to produce all requested sections at full density (subject to Section 2 exception).
- If full density cannot be maintained for the combined request:
  - Explicitly state the limitation.
  - Do not silently reduce density.
  - Propose a practical split.

## 4.14 BIO Contents Requirements (Reader Guide + Ordered Section List)
------------------------------------------
BIO contents MUST include:
- Instructional title and instructor (allowed in contents only; see 4.16).
- Reader Guide stating: “This BIO is ordered for linear reading; proceed top-to-bottom.”
- A single ordered contents list for Sections 1–15 (include Section 15 as optional if used).

## 4.15 Contents-to-Body Heading Matching (UNIVERSAL) (MANDATORY)
------------------------------------------
- Every section heading listed in BIO contents MUST match the body section heading text exactly.
- If a section is regenerated, its heading text must remain identical unless the user explicitly requests a global refactor.

## 4.16 Citations and Source/Instructor Meta (No Meta)
--------------------------------------
- No citations, footnotes, bibliographies, or reference markers by default.
- Transcript-derived sections shall not refer to the instructor/platform/video/course.
- Exception: instructor name is permitted ONLY in BIO contents.
- No meta narration in transcript-derived sections (avoid “In this section…”, “Next we…” style framing).
- Exceptions:
  - Reader Guide inside BIO contents.
  - Section 15 is non-transcript operational guidance and must be [G]-tagged.

## 4.17 Wrapping Rule (Transport-Safe)
--------------------------------------
- Do not manually hard-wrap prose or bullets.
- Only ASCII diagram blocks are hard-wrapped.

## 4.18 No ASCII Framing Inside BIO (MANDATORY)
--------------------------------------
- Inside the BIO document, use markdown headings only.
- Do not use underline framing (e.g., "=====" / "-----") for headings inside BIO content.

## 4.19 Executive Summary Density (Section 2)
--------------------------------------
Section 2 is reduced density:
- Typically 6–10 top-level bullets.
- Shallow nesting (0–2 sub-bullets per top-level bullet).
- Focus on system structure, strategic themes, major decision points.

## 4.20 Heading and Anchor Naming Rules (GitHub Best Practice)
--------------------------------------
- Prefer short, unique noun-phrase headings.
- Avoid punctuation-heavy headings; avoid redundant prefixes.
- Keep headings consistent with BIO contents to maintain stable anchors.

## 4.21 Terminology Standardisation and Alias Rule
--------------------------------------
- If transcript uses multiple terms for the same concept, choose one primary term for use throughout the BIO.
- Record aliases once in Section 13 (Terminology).

## 4.22 Transcript Typo Normalisation Rule (Terminology Only) (MANDATORY)
--------------------------------------
- Applies to terminology labels/names only (technique names, positional names, named grips, named concepts).
- High-confidence correction:
  - Use corrected standard term throughout transcript-derived sections.
  - Record transcript variants as aliases in Section 13.
- Ambiguous term:
  - Preserve transcript term in the body.
  - In Section 13, mark as ambiguous and list plausible candidates without committing.
- Do not ask the user to resolve spelling unless ambiguity prevents faithful interpretation.
- Does not permit adding mechanics/counters/decision rules not present in transcript.

## 4.23 Partial Coverage Handling (Non-Destructive)
--------------------------------------
If transcript-derived content is partial:
- Output only available transcript-derived content.
- Add terminal bullet: "Coverage incomplete due to missing or insufficient transcript content."
Do not invent material.


# 5. FORMATTING REQUIREMENTS
==============================

## 5.1 Transport vs Document Layer
-------------------------------
- Each requested section is returned inside one fenced code block for copy/paste.
- Code fences are transport wrappers only and are not part of the BIO document.

## 5.2 BIO Markdown Heading Templates
-------------------------------
BIO uses markdown headings only:
- Optional Level 1 once: "# [Instructional Title]"
- Level 2 section headers:
  - "## BIO CONTENTS"
  - "## 1.0 MASTER SYSTEM MAP"
  - "## 2.0 EXECUTIVE SUMMARY"
  - …
  - "## 15.0 SUPPLEMENT (NOT TRANSCRIPT-DERIVED)" (optional)
- Level 3: "### {X.Y} {Title Case}"
- Level 4: "#### {X.Y.Z} {Title Case}" when needed


# 6. WORKFLOW
==============================

## 6.1 Start Condition
- User initiates BIO by requesting "BIO contents".

## 6.2 Default Generation Sequence
- Generate in numeric order: BIO contents, then Sections 1–14 (and Section 15 only if requested).

## 6.3 Out-of-Order Section Generation (Permitted With Paste-Location Note)
- If the user requests a section out of order:
  - Include, as the first line inside the code block, a paste-location note:
    - "PASTE AFTER: ## X.0 <Section Name>"
  - Do not include any other meta narration.

## 6.4 Parted Delivery Markers (MANDATORY WHEN USED)
- If a section must be split across multiple responses:
  - Each part repeats the exact same section header at the top.
  - Immediately under the section header, add:
    - "CONTINUED (Part N of M)"
  - End of each part must include exactly one of:
    - "CONTINUES IN PART N+1"
    - "END OF SECTION"


# 7. REQUIRED BIO ARCHITECTURE (UNIFIED ORDER)
=======================================

The BIO MUST be assembled in this exact order:

- BIO CONTENTS
- 1.0 MASTER SYSTEM MAP
- 2.0 EXECUTIVE SUMMARY
- 3.0 VOLUME INDEX
- 4.0 CORE CONCEPTS
- 5.0 SYSTEM OVERVIEW
- 6.0 TECHNIQUE LIBRARY
- 7.0 DIAGRAM SET
- 8.0 APPLICATION SCENARIOS
- 9.0 DRILLING PROGRESSIONS
- 10.0 FOUR-WEEK CURRICULUM
- 11.0 FAILURE PATTERNS
- 12.0 KEY PASSAGES
- 13.0 TERMINOLOGY
- 14.0 ADDITIONAL NOTES
- 15.0 SUPPLEMENT (NOT TRANSCRIPT-DERIVED) (optional)


# 8. SECTION-SPECIFIC RULES
==============================

## 8.1 Section 1 – Master System Map (Macro) (MANDATORY)
- Purpose: macro-level system overview.
- 1–3 ASCII diagrams maximum.
- Must include mandatory legend/conventions block (8.2).
- Must represent:
  - major phases/domains,
  - key positional hubs,
  - major transition families,
  - primary outcome/end-state nodes.

## 8.2 Diagram Legend and Conventions (MANDATORY)
Use these conventions consistently in Section 1 and reuse them in Section 7:
- Hubs: "[HUB]"
- Outcomes/end states: "(OUTCOME)"
- Transitions: "A -> B"
- Primary branching: "{OR}"
- Short arrow labels permitted if transcript provides named links.

## 8.3 Section 7 – Diagram Set (Micro) (MANDATORY)
- Purpose: micro choke-point diagrams that operationalise specific decision gates.
- 5–8 diagrams recommended; cap 10.
- Must not restate Section 1; must expand specific gates/branches.
- Must reuse the same legend/conventions as Section 1.

## 8.4 Section 3 – Volume Index (Mandatory Structure)
- Identify all volumes/chapters.
- Use transcript titles verbatim; if missing, derive concise descriptive volume headers from that volume’s dominant themes only.
- BIO contents entries and Section 3 headers must match exactly.
- Each volume entry includes one sentence (max two) descriptor.

## 8.5 Section 6 – Technique Library (Technique Cards) (MANDATORY)
Every technique entry MUST use Technique Card format with transcript-derived content only:
- Entry condition(s)
- Primary controls
- Structure rules / acceptance criteria
- Opponent main counters (as described)
- Primary continuations
- Abort criteria
- Common failure patterns + correction cues
- End state

## 8.6 Technique Card Sparsity Rule (MANDATORY)
- If a field has no transcript support, OMIT the field.
- If the technique itself has no meaningful transcript-derived detail beyond a label:
  - Output a minimal card with exactly one line:
    - "No transcript-derived content available for this technique."
- Do not invent mechanics.

## 8.7 Technique Library Regrouping Cross-Reference Rule (WHEN USED)
If Section 6 is regrouped by topic-family rather than mirroring Section 3 ordering:
- Each topic-family group heading MUST include a parenthetical cross-reference to relevant volume(s), e.g.:
  - "### 6.X Entries (Vol 1, Vol 3)"
- Individual technique cards may include a short placement line:
  - "- Source volume: Vol X"
Placement reference only; no non-transcript additions.


# 9. SECTION 15 SUPPLEMENT RULES (OPTIONAL)
==============================

## 9.1 Supplement (Not Transcript-Derived) Quarantine (MANDATORY IF USED)
- Section 15 MUST begin with a warning block (2–4 bullets):
  - Not transcript-derived
  - Do not merge into Sections 1–14
  - Every bullet is [G]
- Every bullet in Section 15 MUST begin with "[G]".

## 9.2 Allowed Content Types in Section 15 (CONSTRAINED)
Section 15 may contain ONLY:
- [G] study workflow / viewing strategy
- [G] training templates (constraint games, round structure, progressions)
- [G] safety notes / risk controls
- [G] indexing/search tips for GitHub usage
- [G] audit checklists for Technique Card completeness and usability

Explicitly forbidden in Section 15:
- Technique mechanics, counters, decision trees, or positional specifics not present in transcript (these belong nowhere in transcript-derived BIO and must not be smuggled via [G]).


# 10. EXCEPTION MANAGEMENT
==============================

- Do not invent content to fill missing coverage.
- If a required section has no meaningful transcript-derived content:
  - Output exactly: "No transcript-derived content available for this section."
- If partial coverage exists:
  - Output available content and add:
    - "Coverage incomplete due to missing or insufficient transcript content."


# 11. COMPLIANCE CRITERIA
==============================

[ ] Numbering matches physical reading order (unified order)
[ ] Sections 1–14 are transcript-derived (only permitted synthesis: volume headers; terminology normalisation)
[ ] BIO contents includes Reader Guide and ordered section list
[ ] Contents-to-body headings match exactly
[ ] No ASCII framing inside BIO (markdown headings only)
[ ] Prose/bullets unwrapped; diagrams only hard-wrapped; ≤120 chars/line
[ ] Section 1 macro diagrams (≤3) include mandatory legend/conventions
[ ] Section 7 micro diagrams (cap 10) reuse legend and do not restate Section 1
[ ] Section 6 Technique Cards used; sparsity rule applied; no invented fields
[ ] Section 13 contains terminology aliases/ambiguity entries where applicable
[ ] No citations/footnotes/reference markers
[ ] No instructor/platform/video references in transcript-derived sections (exception: contents only)
[ ] Partial coverage handled without invention
[ ] If Section 15 present: warning block + all bullets [G] + constrained content types only


# 12. OPERATIONAL COMMAND GLOSSARY (USER)
=========================================

"BIO contents"
- Generate BIO contents for the current instructional under this standard.

"Give me Section X"
- Generate exactly Section X (e.g., "Section 6").

"Regenerate Section X"
- Replace the previous version of Section X preserving invariants.

"Out-of-order: Section X"
- Generate Section X and include a paste-location note as the first line inside the code block.


# 13. PRE-OUTPUT LINT CHECKLIST (ASSISTANT)
============================================

- Output is in one fenced code block.
- Only requested section(s) included; no extra preamble.
- No duplicate file-level title after BIO contents.
- Headings use only "#", "##", "###", "####".
- No ASCII framing inside BIO.
- Prose/bullets not hard-wrapped; diagrams only; diagram lines ≤120 chars.
- No citations/footnotes/reference markers.
- No instructor/platform/video references in transcript-derived sections (exception: contents only).
- No meta narration in transcript-derived sections.
- Contents-to-body headings match exactly.
- Section 1 includes legend/conventions; diagrams macro; ≤3 diagrams.
- Section 7 diagrams micro; cap 10; reuse legend; no restatement.
- Section 6 Technique Cards used; sparsity rule applied; regrouping cross-references applied if used.
- Section 13 includes typo normalisation aliases and ambiguity entries where applicable.
- Partial coverage handled without invention and includes terminal coverage line where needed.
- If Section 15 present: warning block present; all bullets begin with "[G]" and content types constrained.


================================================================
END OF DOCUMENT — JIGORO TEXT (BIO INSTRUCTIONS) v6.0
================================================================
