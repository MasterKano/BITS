# Kano Scroll v3.4 — BITS Training Guidance Manual

## 0. Purpose

- Provide a repeatable method to learn and train from grappling instructionals using:
  - `INS/` (per-instructional VN + sessions + transcript/BIO storage)
  - `SYS/` (one unified system library)
- Ensure technical training content is derived from:
  - [I] raw transcript
  - [B] BIO report generated from that transcript
- Enable replication in a new chat with memory off by following the Startup Protocol.

## 1. Definitions

### 1.1 Practitioners

- Assume two medium-to-advanced practitioners.
- Use Person A / Person B only when needed; otherwise partner/opponent.

### 1.2 Sources

- [I] = transcript (raw)
- [B] = BIO (transcript-derived)
- [G] = general knowledge (workflow/process only by default; technical [G] requires explicit request)

### 1.3 Technical vs non-technical

- Technical content: mechanics, positions, grips, transitions, decision rules, prescribed drills/games.
- Non-technical: repo structure, markdown, scheduling, note-taking workflow.

## 2. Non-Negotiables

- One unified Systems library: `SYS/` only.
- No per-instructional duplicate systems folders.
- Technical content must be [I]/[B]-derived unless user explicitly requests technical [G].
- Use short file names and headings; avoid redundant “System – …” labels.

## 3. Repo Structure (BITS)

### 3.1 Top level

- `README.md` = global dashboard (links)
- `Kano-Scroll.md` = this manual
- `INS/` = per-instructional material
- `SYS/` = unified system library
- `standards/` = optional but recommended (stores separate standards such as a BIO generation standard)

### 3.2 Per instructional folder

    INS/<instr>/
      README.md
      bio-<tag>.md
      VN/
      sessions/
      transcripts/

### 3.3 Unified systems

    SYS/<domain>/
      <topic>.md

### 3.4 BIO standard (recommended)

- If you maintain a separate BIO creation standard, store it at:
  - `standards/bio-standard.md`
- Kano Scroll governs training guidance outputs; the BIO standard governs BIO generation outputs.

## 4. Dashboards

- Root `README.md` links to:
  - current active instructional dashboard
  - key unified systems pages
  - Kano Scroll
  - BIO standard (if used)
- `INS/<instr>/README.md` links to:
  - bio, VN, sessions, transcripts
  - relevant unified systems pages

## 5. Workflow

### 5.1 VN (Viewing Notes)

- Location: `INS/<instr>/VN/vX.md`
- Contents: subchapter-structured notes derived from [I]/[B]
- Purpose: study + extraction for sessions and unified system updates

### 5.2 Sessions (per instructional)

- Location: `INS/<instr>/sessions/S01-<tag>.md` … `S12-<tag>.md`
- Purpose: teach the instructional’s system in a structured course
- Session page template:
  - `# Session 0X — <tag> — <theme>`
  - `## Goal`
  - `## Focus`
  - `## Plan (60 min)`
  - `## What worked`
  - `## What to fix next time`

### 5.3 Unified systems updates (promotion rule)

- After reviewing VN or running sessions, promote durable insights into `SYS/`.
- Unified system pages remain concise and navigable:
  - purpose, key positions, entries, cues, offense/defense, drills, errors, notes
- Avoid duplicating entire VN inside systems pages.

### 5.4 BIO role in this workflow

- BIO is a recommended upstream artifact:
  - [I] transcript → [B] BIO → VN / sessions / SYS updates
- BIO is stored per instructional at:
  - `INS/<instr>/bio-<tag>.md`
- If BIO is not available, VN and sessions may be generated directly from [I] (transcript-only mode).

## 6. Links and Anchors

- Use relative markdown links.
- Keep headings short to keep anchor IDs short.
- Use anchors only for high-utility sections (entries, cues, drills).

## 7. Output Rules (assistant behaviour)

These rules exist to keep outputs copy/paste-safe and consistent across new chats:

- All deliverables must be returned in a single fenced code block (markdown).
- The first line of any deliverable must state the target path, e.g.:
  - `PATH: SYS/standup/over-under.md`
  - `PATH: INS/s2g3/sessions/S01-s2g3.md`
- No citations/footnotes. Links are allowed.
- No unnecessary preamble; deliver the requested file content.

## 8. Startup Protocol (new chat, memory off)

To start a new instructional project, provide in this order:

1. Paste `Kano Scroll` (this manual) OR confirm it is the governing standard.
2. Provide the instructional tag + folder name (short), e.g. `s2g3`.
3. Provide:
   - [I] transcript file(s) (txt), and
   - [B] BIO report (md/txt), if available
4. Provide the chapter/subchapter titles + timestamps (paste or txt).
5. Command sequence:
   - `Index: root`
   - `Index: instructional <instr>`
   - `VN <tag> v1`
   - `System <domain>/<topic>`
   - `Session 01 <tag>`
   - Continue as needed.

## 9. Command Cheat Sheet

Common commands (short form):

- `Index: root`
  - Generate content for root `README.md` (global dashboard with links).
- `Index: instructional <instr>`
  - Generate content for `INS/<instr>/README.md` (local dashboard with links).
- `VN <tag> vX`
  - Generate Viewing Notes for volume X (from [I]/[B]).
- `Session 0X <tag>`
  - Generate a session plan for session 0X, stored under the instructional’s sessions folder.
- `System <domain>/<topic>`
  - Generate or update a unified system page under `SYS/<domain>/<topic>.md`.
- `Refactor: headings`
  - Shorten headings and normalize anchor-friendly structure (no content loss).
- `Tag sources: on`
  - Output [I]/[B]/[G] tags on relevant bullets (only when requested).
- `Tag sources: off`
  - Default mode; no source tags.

## 10. Change Control

- “Locked” items (once explicitly locked):
  - session headline list for an instructional
  - repo naming conventions for that project
- To change a locked item, the user must explicitly request the change.

---

End — Kano Scroll v3.4
