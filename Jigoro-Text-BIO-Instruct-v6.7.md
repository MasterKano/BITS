PATH: Jigoro-Text-BIO-Instruct-v6.7.md

# JIGORO TEXT (BIO INSTRUCTIONS) v6.7 (PUBLISHED)

## DOCUMENT INFORMATION

- Document Title: Jigoro Text (BIO Instructions)
- Document Number: JH-MJK-001
- Version: 6.7
- Status: Approved (Published)
- Date of Issue: 2026-01-24
- Supersedes: v6.6
- Issued By: JH
- Maintained By: ChatGPT Execution System

## REVISION HISTORY

- v6.7
  - Added Titles File Authority rules for BIO Section 3.0 (Volume Index) and diagram labeling.
  - Added requirement: Section 3.0 must include per-volume subchapter outline when Titles file exists; otherwise include brief per-volume overview.
  - Added lumped transcript remediation rule for BIO (re-parse embedded subchapters before declaring missing).
  - Added timestamp conflict policy (precedence + handling inconsistent Titles time ranges).
  - Expanded pre-output lint checklist to include Titles-alignment validation for Section 3.0.

---

## 0. OPERATIONAL SUMMARY

- Source of truth: technical content must be transcript-derived.
- BIO Contents is the lock: exact section titles/order are authoritative for this BIO.
- Reader order is physical order: the BIO is written and read in the same sequence.
- Titles file authority (when provided): governs Volume Index outlines and diagram labeling (see 5.3, 7.4).
- Wrapping: no manual hard-wrap except ASCII diagrams (≤120 chars/line).
- Supplement boundary: only Section 15 may be non-transcript-derived and must be explicitly marked.
- Output reliability rule: if output limits are hit, the assistant must safe-stop at a declared boundary and provide a resume token.

---

## 1. SCOPE

This standard defines how to convert any BJJ instructional transcript into a single logical BIO markdown document delivered in parts, using the locked reader-order section template in Section 7.

---

## 2. DEFINITIONS

- Transcript-derived: content originates strictly from transcript text, with minimal clarity edits and permitted title synthesis where transcript lacks explicit titles.
- Deep Density: encode conditions, decision forks, constraints, sequencing, failure patterns and corrections when present; avoid filler and non-transcript technical additions.
- ASCII Width Rule: diagrams ≤120 characters per line; only diagrams may be hard-wrapped.
- Lock scope: the locked template constrains section titles/order; it does not cap the number of transcript-driven sub-chapters.
- Safe-stop: a mandatory stop at a named boundary when output length constraints are reached.
- Titles file: a separate outline artifact listing official chapter/subchapter headings (and sometimes time ranges).

---

## 3. GENERAL REQUIREMENTS

- No unnecessary questions; proceed best-effort unless transcript is missing/corrupt/unreadable or a mandatory output cannot be populated without invention.
- No instructor/platform/video meta narration.
- Bullets use "-" with consistent indentation (nested hyphen lists).
- Do not invent technical content. If unknown/absent, flag it explicitly.

---

## 4. FORMATTING RULES

- All deliverables returned in a single fenced code block for copy/paste (transport only).
- BIO uses markdown headings only (up to four levels).
- No manual hard-wrapping for prose/bullets; diagrams only are hard-wrapped to comply with ASCII Width Rule.
- Transport markers are mandatory only when batching/chunking (Section 6.4). Single-section delivery does not require wrappers.

---

## 5. WORKFLOW RULES

- A new BIO begins when the user requests BIO Contents (or explicitly starts a new BIO).
- BIO Contents is produced first and becomes the lock for:
  - section existence,
  - exact header text,
  - “Next” progression,
  - regeneration invariants.

### 5.1 Transcripts without timestamps (segmentation rule)

If the transcript lacks timestamps or chapter markers:
- Segment by topic shifts (new position, new submission family, new major defence tree, or a new drill/curriculum block).
- Record segmentation assumptions in:
  - Section 14.0 Additional Notes
- Do not invent technical content to “fit” a segment; segmentation is editorial structure only.

### 5.2 LOCKED scope clarification (critical)

- LOCKED applies to:
  - Section titles and numbering in Section 7.1
  - Locked physical order
  - Command semantics (Section 6)
- LOCKED does not apply to:
  - The number of sub-chapters inside a section (e.g., 6.1–6.n)
  - Transcript-driven expansion needed to represent the instructional faithfully
- If a tool/UI claims “cannot expand locked sections”, treat that as a delivery-size constraint problem and use Section 6 chunking/range commands.

### 5.3 Titles file authority (mandatory when provided)

If a Titles file exists for the instructional:
- Titles is the controlling authority for:
  - Section 3.0 Volume Index subchapter outlines (see 7.4)
  - diagram naming/labeling in Section 7.0 (volume/subchapter labels)
- Transcript-derived segmentation is subordinate:
  - if transcript text is merged/lumped, re-parse to match Titles subchapters before declaring “missing.”

### 5.4 Lumped transcript remediation (required)

When transcript text merges multiple titled subchapters into a single paragraph/block:
- First assume missing material is embedded nearby.
- Re-parse by instructional signals in this order:
  1) stated purpose (“today we will…”)
  2) opponent reaction / defensive response
  3) corrective rule / constraint
  4) hub/position change
- Extract and relocate into the correct Titles subchapter(s) or BIO outline bullets.
- Only after a targeted scan may you declare “missing content,” and you must name the missing item.

### 5.5 Timestamp conflict policy

- Timecodes are optional; include only when they materially reduce ambiguity.
- Precedence:
  1) transcript timecodes (highest)
  2) Titles file time ranges
  3) none
- If Titles time ranges are inconsistent/non-linear:
  - keep them as labels only
  - preserve Titles order (do not reorder content to “fit” timestamps)
  - optionally add a single note in Section 14.0 Additional Notes

---

## 6. COMMAND SEMANTICS (LOCKED)

### 6.1 Single-step commands (baseline)

- “BIO Contents”
  - Output the BIO Contents for the current instructional using the locked template in Section 7.
- “Next”
  - Output the next section in the locked BIO order as defined by the current BIO Contents.
- “Section X”
  - Output exactly Section X (only if it exists in the locked BIO Contents for this BIO).
- “Regenerate Section X”
  - Replace Section X while preserving numbering, header text, and ordering as locked by BIO Contents.

### 6.2 Batch commands (multi-step, locked order)

Batch commands reduce repetitive “Next” interactions while preserving the locked order.

Supported forms:
- “Next xN”
  - Output the next N sections in locked order.
- “Batch: BIO Contents; Next xN”
  - Run multiple commands in sequence (executed strictly left-to-right).

Mandatory safe-stop behavior:
- If output length constraints are hit mid-batch:
  - stop at the end of the last fully completed section (or chunk boundary, if chunking is active),
  - state exactly which section is next,
  - provide a resume token (see 6.5),
  - user resumes with “Resume <token>” or “Next” or another batch/range command.

### 6.3 Range commands (preferred for predictability)

Supported forms:
- “Sections A-B”
  - Output sections A through B inclusive, in locked order.
- “Sections A-B xParts”
  - Output sections A through B but allow safe-stop and continuation until the entire range is complete.
- “Sections A-B (Parts)”
  - Alias of xParts.
- “Section X (Parts)”
  - Alias of “Section X” with safe-stop/resume until the full section is delivered.

### 6.4 Chunking commands (for large sections)

Supported forms:
- “Section X chunked”
  - Assistant chooses chunk boundaries at subchapter boundaries and safe-stops between chunks.
- “Section X chunked by Y”
  - Example: “Section 6.0 chunked by 3 subchapters”
- “Section X.Y-Z”
  - Output a subchapter range only (inside Section X).

Transport markers (mandatory when batching or chunking):
- Each delivered section must be wrapped as:

  BEGIN SECTION 6.0
  <content>
  END SECTION 6.0

- Each delivered chunk must be wrapped as:

  BEGIN CHUNK 6.4-6.6
  <content>
  END CHUNK 6.4-6.6

These markers are transport only; they do not change the BIO’s internal headings.

### 6.5 Resume protocol (mandatory)

If a safe-stop occurs, the assistant must output:
- NEXT: <the next section/chunk boundary>
- RESUME TOKEN: RESUME:<section-or-chunk>

User resumes with:
- “Resume RESUME:<section-or-chunk>”
- Or a new command starting at that point.

### 6.6 Deterministic stop-after option (user-controlled)

User may specify:
- “Sections A-B; stop after Section K”
- “Next xN; stop after Section K”

Rule:
- The assistant must stop at the declared boundary even if additional output capacity remains.

### 6.7 Recommended batch sizing (best-effort guidance)

- Prefer “Sections 1-3 (Parts)” for initial delivery.
- Prefer “Section 6.0 chunked” for Technique Library when dense.
- Prefer 1–2 sections per response for diagram-heavy portions (7.0+) unless using (Parts).

---

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
- Diagram lines ≤120 chars; diagrams may be hard-wrapped; non-diagram text must not be hard-wrapped.

### 7.4 Volume Index requirement (Section 3)

Section 3.0 must represent each volume in a way that is useful and outline-faithful:

- If a Titles file exists:
  - Each volume entry (3.1, 3.2, …) must include, at minimum, the Titles-file subchapter list for that volume.
  - Titles wording is controlling (minor punctuation normalization allowed).
- If no Titles file exists:
  - Each volume entry must include either:
    - a concise subchapter list derived from transcript segmentation, or
    - a brief 1–3 bullet overview of what the volume covers (minimum).

---

## 8. INCOMPLETE COVERAGE HANDLING (STRICT)

- Never invent content.
- If something is missing, state exactly what is missing (e.g., missing transcript for a titled subchapter, missing volume transcript, missing timestamp block).
- Do not use generic “coverage incomplete…” lines without specifying the missing item.
- Before declaring missing subchapters, apply lumped transcript remediation (5.4).

---

## 9. TRANSCRIPT TYPO NORMALIZATION (TRACEABLE)

- Do not silently rename techniques in transcript-derived sections.
- If a token appears incorrect, keep the transcript token and add the normalized name in a traceable way (e.g., “Choi bar (transcript: ‘troy bar’)”).
- Maintain these mappings in Section 13 (Terminology) and/or Section 15 (Supplement), as appropriate.

---

## 10. SUPPLEMENT BOUNDARY (SECTION 15 ONLY)

- Only Section 15 may include non-transcript-derived content.
- Every non-transcript-derived bullet must begin with “(SUPPLEMENT)”.

---

## 11. PRE-OUTPUT LINT CHECKLIST (ASSISTANT)

- Output matches locked section names/order from BIO Contents.
- Section 1.0 is an ASCII diagram at the top of the report and complies with width rules.
- Section 3.0 satisfies the Volume Index requirement (7.4) and is Titles-aligned when Titles exists.
- No legacy Annex/Appendix structures unless explicitly present in the locked BIO Contents (prohibited by default).
- No hard-wrapping except ASCII diagrams; diagram width ≤120 chars/line.
- No meta narration; no non-transcript technical content outside Section 15.
- If missing content is flagged, it explicitly names what is missing and follows lumped remediation first.
- If safe-stop occurs, provide NEXT + RESUME TOKEN per Section 6.5.

END OF JIGORO TEXT (BIO INSTRUCTIONS) v6.7
