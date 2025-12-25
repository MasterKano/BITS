# JIGORO TEXT (BIO INSTRUCTIONS) v6.2

## DOCUMENT INFORMATION

- Document Title: Jigoro Text (BIO Instructions)
- Document Number: JH-MJK-001
- Version: 6.2
- Status: Approved
- Date of Issue: 2025-12-25
- Supersedes: v6.1
- Issued By: JH
- Maintained By: ChatGPT Execution System

## REVISION HISTORY

- v6.2
  - Locked the reader-order BIO template where 1.0 is Master System Map (ASCII), 2.0 is Executive Summary, 3.0 is Volume Index.
  - Removed the requirement for a separate Structure Manifest by making BIO Contents the single authoritative “lock” (headers + order).
  - Added hard rule: “Next” advances strictly by the locked BIO Contents order (no legacy templates, no annex/appendix leakage).
  - Added Section 11 (Failure Patterns) and Section 12 (Key Passages) as required sections.
  - Reaffirmed: sub-chapters are transcript-customized inside each section; section numbering/titles remain fixed.

## 0. OPERATIONAL SUMMARY

- Source of truth: technical content must be transcript-derived.
- BIO Contents is the lock: exact section titles/order are authoritative for this BIO.
- Reader order is physical order: the BIO is written and read in the same sequence.
- Wrapping: no manual hard-wrap except ASCII diagrams (≤120 chars/line).
- Supplement boundary: only Section 15 may be non-transcript-derived and must be explicitly marked.

## 1. SCOPE

This standard defines how to convert any BJJ instructional transcript into a single logical BIO markdown document delivered in parts, using the locked reader-order section template in Section 7.

## 2. DEFINITIONS

- Transcript-derived: content originates strictly from transcript text, with minimal clarity edits and permitted title synthesis where transcript lacks explicit titles.
- Deep Density: encode conditions, decision forks, constraints, sequencing, failure patterns and corrections when present; avoid filler and non-transcript technical additions.
- ASCII Width Rule: diagrams ≤120 characters per line; only diagrams may be hard-wrapped.

## 3. GENERAL REQUIREMENTS

- No unnecessary questions; proceed best-effort unless transcript is missing/corrupt/unreadable or a mandatory output cannot be populated without invention.
- No instructor/platform/video meta narration.
- Bullets use "-" with consistent indentation (nested hyphen lists).

## 4. FORMATTING RULES

- All deliverables returned in a single fenced code block for copy/paste (transport only).
- BIO uses markdown headings only (up to four levels).
- No manual hard-wrapping for prose/bullets; diagrams only are hard-wrapped to comply with ASCII Width Rule.

## 5. WORKFLOW RULES

- A new BIO begins when the user requests BIO Contents (or explicitly starts a new BIO).
- BIO Contents is produced first and becomes the lock for:
  - section existence,
  - exact header text,
  - “Next” progression,
  - regeneration invariants.

## 6. COMMAND SEMANTICS (LOCKED)

- “BIO Contents”
  - Output the BIO Contents for the current instructional using the locked template in Section 7.
- “Next”
  - Output the next section in the locked BIO order as defined by the current BIO Contents.
- “Section X”
  - Output exactly Section X (only if it exists in the locked BIO Contents for this BIO).
- “Regenerate Section X”
  - Replace Section X while preserving numbering, header text, and ordering as locked by BIO Contents.

## 7. REQUIRED BIO ARCHITECTURE (LOCKED TEMPLATE)

### 7.1 Locked section order (physical = reading order)

- 1.0 MASTER SYSTEM MAP (ASCII)
- 2.0 EXECUTIVE SUMMARY
- 3.0 VOLUME INDEX
  - 3.1 Volume 1 — [Transcript-custom title]
  - 3.2 Volume 2 — [Transcript-custom title]
  - 3.3 Volume 3 — [Transcript-custom title]
  - (extend as needed for all volumes)
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
- 15.0 SUPPLEMENT (NOT TRANSCRIPT-DERIVED) (OPTIONAL)

### 7.2 Customization rule (sub-chapters)

- Section titles and numbering above are fixed.
- Sub-chapters inside sections (e.g., 4.1, 5.2, 6.3, 8.4, etc.) must be customized to the transcript/instructional content.
- Volume Index sub-entries (3.1, 3.2, …) must exist for every volume provided; naming must be transcript-faithful (or minimally synthesized if the transcript lacks explicit titles).

### 7.3 Master System Map requirement (Section 1)

- Section 1 must be ASCII diagram(s) plus any minimal supporting text needed for correct reading/use.
- Diagrams must be transcript-derived in node/transition selection (no speculative nodes).
- Diagram lines ≤120 chars; diagrams may be hard-wrapped, non-diagram text must not be hard-wrapped.

## 8. INCOMPLETE COVERAGE HANDLING (STRICT)

- Never invent content.
- If something is missing, state exactly what is missing (e.g., missing transcript for a titled subchapter, missing volume transcript, missing timestamp block).
- Do not use generic “coverage incomplete…” lines without specifying the missing item.

## 9. TRANSCRIPT TYPO NORMALIZATION (TRACEABLE)

- Do not silently rename techniques in transcript-derived sections.
- If a token appears incorrect, keep the transcript token and add the normalized name in a traceable way (e.g., “Choi bar (transcript: ‘troy bar’)”).
- Maintain these mappings in Section 13 (Terminology) and/or Section 15 (Supplement), as appropriate.

## 10. SUPPLEMENT BOUNDARY (SECTION 15 ONLY)

- Only Section 15 may include non-transcript-derived content.
- Every non-transcript-derived bullet must begin with “(SUPPLEMENT)”.

## 11. PRE-OUTPUT LINT CHECKLIST (ASSISTANT)

- Output matches locked section names/order from BIO Contents.
- No legacy Annex/Appendix structures unless explicitly present in the locked BIO Contents (prohibited by default).
- No hard-wrapping except ASCII diagrams; diagram width ≤120 chars/line.
- No meta narration; no non-transcript technical content outside Section 15.
- If missing content is flagged, it explicitly names what is missing.

END OF JIGORO TEXT (BIO INSTRUCTIONS) v6.2
