PATH: SYS/Guard/Open-Guard/open-guard_master-operating-system.md

# Open Guard — Master Operating System (Controller)

## 1. Purpose
A controller system for Open Guard that:
- prevents passing by denying pass-building requirements early, and
- converts every successful defensive cycle into immediate counter-offense.

This page defines the master loop, gates, selection rules, and failure diagnostics. All Open Guard sub-systems plug into this.

## 2. Canonical Loop (non-negotiable)
**READ → CONNECT → DENY → RECENTER → (BASE BREAK → ENTER → STABILIZE → FINISH) OR (DEFENSIVE CYCLE)**

- **READ:** opponent intent + commitment (energy + posture context)
- **CONNECT:** establish a true handle + redundancy (hands + feet)
- **DENY:** break the pass requirement currently being built (not “a pass”)
- **RECENTER:** restore alignment (opponent in front, barriers between bodies)
- **BASE BREAK:** force posting / widened base (validity for entries)
- **ENTER:** choose the lowest-complexity entry that matches range + posture
- **STABILIZE:** land in a hub that suppresses the opponent’s best exit
- **FINISH:** submit/sweep/top without allowing reset
- **DEFENSIVE CYCLE:** mandatory when hip line is threatened (see Gate A)

## 3. Master Gates (these override everything)

### 3.1 Gate A — Hip Line Gate (phase switch)
**Question:** Is the opponent at/past your hip line?

- **NO (in front of hip line):**
  - mobility solutions dominate (pummel/crossover/pendulum/scoot)
  - objective: keep them in front; deny angle before penetration
- **YES (at/past hip line):**
  - you are in **DEFENSIVE CYCLE**
  - frames become structural; re-align before any “offense”
  - objective: rebuild barriers + recover facing until cycle break

**Cycle break definition (must satisfy all):**
- opponent re-centered (no dominant angle)
- barriers rebuilt (legs/frames between bodies)
- orientation restored (feet or knees facing)
- hip line no longer threatened

### 3.2 Gate B — Hands-Down Gate (entry validity)
**Question:** Is their base truly compromised (posting/hands-down/widened base)?

- **NO (upright stable base):**
  - keep off-balancing; keep connection
  - do **not** spin/rotate under stable posture
- **YES (base compromised):**
  - entry window is open; commit to entry/hub

### 3.3 Gate C — Orientation Rule (retention integrity)
At all times:
- **feet or knees must face the opponent**
- if one is displaced, the other replaces it immediately
- “double loss” (neither facing) is a red alarm: angle → penetration → hip line follows

## 4. Passing Model (what you defend)
Passing is a requirements chain:
**Distance → Grip → Angle → Level → Penetration → Pin**

Retention job:
- identify which link is being built now,
- break one link early,
- re-center and rebuild barriers,
- then counter immediately on cycle break.

## 5. Range + Context Selectors (fast rules)
Use these to avoid wrong-family responses:

### 5.1 Energy Read (commitment)
- forward push = protect hip line; deny distance/level
- backward pull = anti-exit; follow; containment if entangled

### 5.2 Context Laws (posture)
- **Kneeling:** shoulders vs hips (base-break window vs withdrawal)
- **Standing:** toes vs heels (drive-in vs backstep/disengage)
- **Head height:** head high → legs; head low → arms/head + go-behind

(Details live in the decision-model SYS files; this controller defines how they plug in.)

## 6. Entry Families (selection by range)
Do not “choose your favorite.” Choose what matches the moment.

- **Distance:** 2-on-1 ankle / partial inversion connectors / shin-to-shin
- **Kneeling:** single/double/reverse double; cross-catch → hip pin
- **Standing bridges:** X-guard / RDLR / HQ (must satisfy hands-down gate)

## 7. Hub Selection (stabilize before finishing)
Hub choice is governed by the opponent’s best exit:

- **Forward pressure / drive-in:** inside senkaku (forward barrier value)
- **Turn-away / disengage:** 50–50 / double 50 (containment)
- **Backside flattening pressure:** criss-cross (backside stability + breaking alignment)

## 8. Exit Governance (no free reset)
Assume the opponent’s primary defense is **reset**, not “fight in place.”

Common exits/defenses:
- backstep
- flee the mat / hard retreat
- heavy leg
- high leg
- leg closure (deny wedge/knee line)
- backside flattening (hands push shoulders flat)

Default counters:
- maintain redundant attachment (disengagement must be slow)
- occupy space (remove ankle gaps; deny leg closure)
- backside is a pushing contest: legs must out-push hands

## 9. Failure Signatures → Fix Rules
- **Late defense (framing after penetration):** hip line gate ignored → escalate earlier
- **Dead feet (touch without control):** no true barrier/hook → pummel with purpose; reconnect feet-first
- **Hand chasing:** arms lead, hips lag → re-square first; hands reinforce structure
- **Spin under stable base:** hands-down gate violated → base-break longer before rotations
- **Thin entries (one step clears):** no true handle → secure ankle/heel line before climbing
- **Stop-pass-stop:** cycle break without counter → apply Golden Rule immediately

## 10. Minimal Drill Ladder (controller-level)
- **Phase 1:** identify which pass link is being built (call it out live)
- **Phase 2:** hip line gate drills (recognize + switch to defensive cycle instantly)
- **Phase 3:** hands-down gate drills (no entry allowed until base compromised)
- **Phase 4:** cycle-break → immediate counter rounds (score only after counter starts)

## 11. Master Diagram (ASCII)

```text
┌──────────────────────────── OPEN GUARD — MASTER CONTROLLER ────────────────────────────┐
│ READ -> CONNECT -> DENY -> RECENTER -> (BASE BREAK -> ENTER -> HUB -> GOVERN EXITS)     │
│                         \-> if HIP LINE THREAT -> DEFENSIVE CYCLE -> CYCLE BREAK -> COUNTER │
└────────────────────────────────────────────────────────────────────────────────────────┘

READ (energy + posture law)
  |
CONNECT (true handle + redundancy)
  |
DENY (break pass-chain link: Distance/Grip/Angle/Level/Penetration/Pin)
  |
RECENTER (opponent in front + barriers rebuilt + orientation restored)
  |
GATE A: HIP LINE THREAT?
  |NO ---------------------------------------------------------------+
  |                                                                   |
  |YES -> DEFENSIVE CYCLE (frames high/low + turn-to-side + shrimp)   |
  |        -> rebuild barriers -> RECENTER -> CYCLE BREAK -> COUNTER  |
  |                                                                   |
  +-------------------------------------------------------------------+
                          |
                          v
BASE BREAK (off-balance)
  |
GATE B: HANDS DOWN?
  |NO -> keep off-balancing (no spin/rotation under stable base)
  |YES-> ENTER (range-appropriate) -> HUB (suppress best exit)
                                   -> EXIT GOVERNANCE (backstep/flee/heavy/high/closure/backside)
                                   -> FINISH or RECYCLE