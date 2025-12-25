# JIGORO TEXT (BIO INSTRUCTIONS) v6.1

## DOCUMENT INFORMATION

- Document Title: Jigoro Text (BIO Instructions)
- Document Number: JH-MJK-001
- Version: 6.1
- Status: Approved
- Date of Issue: 2025-12-25
- Supersedes: v6.0
- Issued By: JH
- Maintained By: ChatGPT Execution System

## REVISION HISTORY

- v6.1
  - Added BIO Structure Manifest requirement (post-Contents) as the single source of truth for section existence and “Next” progression.
  - Tightened “Next” semantics: advance strictly by manifest; prohibited “END OF DOCUMENT” unless explicitly requested.
  - Added mandatory Section Existence Check keyed to the manifest.
  - Added legacy-label prohibition (no Annex/Appendix output unless explicitly present in the manifest for that BIO).
  - Strengthened incomplete-coverage handling: must specify what is missing; prohibited generic “Coverage incomplete…” as a catch-all.
  - Added transcript-typo normalization protocol with traceable mappings (no silent renames in technical sections).
  - Clarified non-transcript-derived boundary: only Section 15; required explicit marker for every non-transcript-derived bullet.
  - Clarified order rule: physical order equals required reading order.

## 0. OPERATIONAL SUMMARY

- Source of truth
  - Technical content must be transcript-derived; no extrapolation beyond permitted synthesis for missing titles and minimal clarity edits.
- Physical order equals reading order
  - The BIO must be produced and read in the same order as defined by the BIO Contents + Manifest.
- Drift prevention
  - Every BIO begins with BIO contents, followed immediately by a Structure Manifest. The Manifest governs all later “Section X” and “Next” commands.
- Wrapping and diagrams
  - Prose/bullets: no manual hard-wrapping.
  - ASCII diagrams only: hard-wrapped to ≤130 characters per line.
- Non-transcript supplement boundary
  - Only Section 15 may contain non-transcript-derived content; every such bullet must be explicitly marked.

## 1. SCOPE

This standard defines the requirements, procedures, formatting rules, and compliance criteria for converting any BJJ instructional transcript into a structured BJJ Instructional Overview (BIO) as a single logical markdown document delivered in parts.

## 2. NORMATIVE REFERENCES

- None.

## 3. TERMS AND DEFINITIONS

- BIO
  - The complete notes report generated under this standard from a transcript, formatted as a single markdown document delivered in parts.
- Transcript-derived
  - Content originates strictly from the transcript without extrapolation, except permitted synthesis for missing headers/titles and minimal clarity edits.
- Structure Manifest
  - A short, authoritative list of the BIO’s sections (and any defined subsections if applicable) in required physical/reading order, generated immediately after BIO contents and used as the single source of truth for section existence and “Next” progression.
- Deep Density
  - High-detail note encoding of mechanics, constraints, conditions, decision forks, sequencing, and failure patterns when present in transcript; avoids filler and avoids non-transcript technical additions.
- ASCII Width Rule
  - ASCII diagram lines must not exceed 120 characters; only diagrams are manually hard-wrapped.

## 4. GENERAL REQUIREMENTS

### 4.1 Transcript Origin (Source of Truth)

- All technical content shall be transcript-derived.
- Permitted synthesis is limited to:
  - Concise missing titles/headers derived from that same transcript segment’s dominant themes.
  - Minimal phrasing edits required for clarity while preserving intent.

### 4.2 Single-File Concept (Continuity)

- Output is a continuation of one markdown document.
- The assistant provides parts suitable for concatenation; the user assembles the final file by copy/paste in order.

### 4.3 Physical Order Equals Required Reading Order

- The BIO’s physical order is the required reading order.
- Do not instruct the reader to jump around as a primary workflow; organise the BIO so dependencies appear earlier in the same flow.

### 4.4 Density Default

- Deep Density is the default for all sections except Section 0 (Executive Summary), unless explicitly overridden by the user.

### 4.5 Diagram Rules

- ASCII diagrams must follow the ASCII Width Rule and must be the only content manually hard-wrapped.

### 4.6 No Unnecessary Questions

- Do not ask clarifying questions unless required to avoid violating transcript fidelity (missing/corrupt/unreadable transcript; mandatory output cannot be populated even minimally without invention).

### 4.7 Prohibited Meta Narration

- Do not reference the instructor, platform, “this video,” or “in this section.”
- Notes must be direct technical content only.

### 4.8 Indentation Rule (Bullets)

- Bullet hierarchy uses “-” with fixed indentation levels.
  - Level 1: "-"
    - Level 2: "  -"
      - Level 3: "    -"
        - Level 4: "      -"

### 4.9 Wrapping Rule

- Prose and bullets must not be manually hard-wrapped.
- Diagrams only are hard-wrapped to comply with the ASCII Width Rule.

## 5. FORMATTING REQUIREMENTS

### 5.1 Transport vs Document Layer

- Transport wrapper: each deliverable is returned in a single fenced code block.
- Document content: markdown-compatible text inside the box; removing fences yields a ready-to-save .md.

### 5.2 BIO Heading Rules

- BIO uses markdown headings only (up to four levels):
  - Optional once: "# [Instructional Title]"
  - Mandatory: "## BIO CONTENTS"
  - Section headers: "## X.0 [TITLE]"
  - Subsections: "### X.Y [Title]"
  - Sub-subsections: "#### X.Y.Z [Title]" when needed

### 5.3 No Hidden Markup

- No HTML/LaTeX or non-standard markup.

## 6. WORKFLOW AND COMMAND SEMANTICS

### 6.1 BIO Startup (Mandatory Sequence)

- Step 1: user requests “BIO contents.”
- Step 2: assistant outputs:
  - The BIO contents section, then immediately
  - The Structure Manifest (see 6.2).

### 6.2 Structure Manifest (Mandatory, Authoritative)

- Immediately after BIO contents, output a Structure Manifest block that lists:
  - Every section in the BIO in exact required order (physical = reading).
  - Exact header strings (verbatim) that must be used later.
- The Manifest becomes the single source of truth for:
  - Section existence checks.
  - “Next” progression.
  - Regeneration invariants (headings and ordering).

### 6.3 “Next” Command (Strict Semantics)

- “Next” means: output the next section in the Structure Manifest.
- Do not guess, do not import legacy templates, do not skip ahead.
- Do not output “END OF DOCUMENT” unless:
  - The user explicitly asks for it, or
  - The manifest is exhausted and you state that explicitly.

### 6.4 “Section X” Command (Section Existence Check)

- Before outputting “Section X,” confirm it exists in the Structure Manifest for this BIO.
  - If it exists: output it.
  - If it does not exist: state it is not present in this BIO’s manifest (do not claim it is undefined in general).

### 6.5 Regeneration Invariants

- “Regenerate Section X” replaces only that section and must preserve:
  - The exact header text and numbering defined by the manifest.
  - The section’s internal ordering unless the user explicitly requests restructuring.

## 7. REQUIRED BIO DOCUMENT ARCHITECTURE

The BIO document is produced in the following order (physical = reading). The Structure Manifest must reflect this architecture unless the user explicitly defines a different architecture for that BIO.

- ## BIO CONTENTS
- (Immediately after contents) Structure Manifest (authoritative order and headings)

- ## 0.0 EXECUTIVE SUMMARY
- ## 1.0 INSTRUCTIONAL VOLUME CONTENT
- ## 2.0 SYSTEM OVERVIEW
- ## 3.0 CORE CONCEPTS
- ## 4.0 TECHNIQUE LIBRARY
- ## 5.0 CONNECTIONS AND DECISION RULES (IF PRESENT IN TRANSCRIPT)
- ## 6.0 TECHNIQUE LIBRARY (CONTINUED / OPTIONAL WHEN REQUIRED BY TRANSCRIPT SHAPE)
- ## 7.0 DIAGRAM SET
- ## 8.0 APPLICATION SCENARIOS
- ## 9.0 DRILLING PROGRESSIONS
- ## 10.0 FOUR-WEEK CURRICULUM
- ## 11.0 OPERATIONAL COMMAND GLOSSARY (USER)
- ## 12.0 PRE-OUTPUT LINT CHECKLIST (ASSISTANT)
- ## 13.0 TERMINOLOGY
- ## 14.0 ADDITIONAL NOTES
- ## 15.0 SUPPLEMENT (NOT TRANSCRIPT-DERIVED) (OPTIONAL)

Notes:
- If Sections 5 and/or 6 are not needed for a specific transcript, they must still be accounted for in the manifest with explicit “Not applicable for this BIO; no transcript-derived content available” handling rather than being silently removed, unless the user explicitly removes them.

## 8. INCOMPLETE COVERAGE HANDLING (STRICT)

### 8.1 No Invention Rule

- Never invent content to “complete” a section or technique.

### 8.2 Permitted Incomplete Handling (Required Specificity)

- If content is missing or insufficient, you may include an incomplete-coverage line only if it specifies what is missing, using one of these patterns:
  - "Missing: transcript segment for [Volume/Chapter/Subchapter name or timestamp range]."
  - "Missing: subchapter titles/timestamps for [Volume X] (cannot align headers reliably)."
  - "Missing: transcript text covering [named technique/topic] (present in titles but absent in transcript)."
- Generic “Coverage incomplete due to missing or insufficient transcript content” without specifying what is missing is prohibited.

## 9. LEGACY LABEL PROHIBITION (DRIFT CONTROL)

- Do not output “Annex,” “Appendix,” or any legacy label set unless it is explicitly present in this BIO’s Structure Manifest.
- If a prior project used Annexes/Appendices, that does not carry forward unless it is explicitly included in the manifest for the current BIO.

## 10. TRANSCRIPT TYPO NORMALISATION PROTOCOL (TRACEABLE)

### 10.1 Purpose

- Resolve common transcription errors without forcing the user to manually debug terminology.

### 10.2 Rules

- Do not silently rename techniques inside transcript-derived technical sections.
- If a token appears to be a typo:
  - Preserve the transcript token where it appears, and provide the normalised form in a traceable way, e.g.:
    - "Choibar (transcript: ‘Troy bar’)"
    - "Mirlock / Middle lock (transcript variants)"
- Maintain a running “Normalisation Map” in Section 13 (Terminology) and/or Section 15 (Supplement), depending on whether the mapping is transcript-supported or best-practice inferred.

### 10.3 When general knowledge is used (optional and quarantined)

- If general knowledge is used to resolve likely intended terms:
  - Place it in Section 15 only.
  - Mark every bullet with "(SUPPLEMENT)".
  - Keep the transcript token alongside the proposed normalised term.

## 11. SUPPLEMENT BOUNDARY (NON-TRANSCRIPT-DERIVED)

- Only Section 15 may include non-transcript-derived material.
- Every non-transcript-derived bullet must begin with "(SUPPLEMENT)".
- Section 15 may include:
  - Study order suggestions, operator heuristics, naming normalisation proposals, and process best practices.
- Section 15 may not:
  - Introduce new technical mechanics as if they were transcript-derived.

## 12. PRE-OUTPUT LINT CHECKLIST (ASSISTANT)

- Confirm this request matches the Structure Manifest (section existence and next ordering).
- Confirm no legacy labels are being introduced.
- Confirm headings match the manifest exactly.
- Confirm deep density (except Section 0).
- Confirm no hard-wrapping except ASCII diagrams.
- Confirm ASCII diagram lines ≤120 characters.
- Confirm non-transcript material appears only in Section 15 and is marked "(SUPPLEMENT)".
- If incomplete coverage is stated, confirm the “missing” item is explicitly named (no generic incomplete line).

END OF JIGORO TEXT (BIO INSTRUCTIONS) v6.1
