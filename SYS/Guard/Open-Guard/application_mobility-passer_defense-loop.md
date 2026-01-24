PATH: SYS/Guard/Open-Guard/application_mobility-passer_defense-loop.md

# Application — Mobility Passer Defense Loop (Open Guard)

## 1. Purpose
An application profile for defending a **mobility passer**: someone who prioritizes circling, shucking legs, and resetting rather than sustained compression.

Goal: keep the passer in front, prevent outside knee line progression, and convert their retreat/reset patterns into attachment + counter windows.

## 2. Inputs / Preconditions
- You can re-square hips quickly (crossover/scoot/pendulum).
- You can reinsert barriers when legs are shucked (foot pummel).
- You can maintain at least light contact and upgrade to a true handle (ankle/heel line).

## 3. Outputs / Success Criteria
- Passer stays **in front** (outside knee line denied).
- You can **prevent disengage** to two steps.
- You force repeated **re-steps** and **re-squares** (they can’t build angle).
- You create a counter start: ankle/heel line true handle or base event.

## 4. Core Model / Engine

### 4.1 Mobility Passer (operational definition)
A mobility passer is identified by:
- frequent lateral circling,
- shove-to-clear patterns,
- backstep/retreat resets,
- low commitment to forward+push pressure.

Primary threat is **Angle** then **Reset**, not Penetration.

### 4.2 Defense Loop (repeatable)
**REINSERT → RE-SQUARE → RE-CENTER → REATTACH → RESTRICT EXIT**

- **REINSERT:** get barriers back inside (legs between bodies).
- **RE-SQUARE:** hips face opponent; deny outside knee line.
- **RE-CENTER:** opponent back in front, not around the corner.
- **REATTACH:** upgrade to true handle (ankle/heel line) + redundancy.
- **RESTRICT EXIT:** prevent backstep/disengage and force them to re-engage.

### 4.3 Domain Progression Chain Hooks (mobility profile)
Mobility passer tends to attack these links:
- **Barrier removal (Distance)** → **Angle** → **Reset**
So your denial focus is:
- reinsertion first, then re-square, then attachment that prevents reset.

## 5. Gates (override rules)

### 5.1 Orientation Rule (primary)
Feet or knees face the opponent.

**Default action:** crossover/scoot immediately when outside knee line is forming.

### 5.2 Hip Line Gate
If hip line is threatened, you are no longer in mobility profile; switch to defensive cycle.

**Default action:** frames high/low → turn-to-side → shrimp → rebuild → re-square.

### 5.3 Hands-Down Gate (commitment)
No committed rotations/entries under stable base.

**Default action:** base-break or attach ankle line first; commit only after base event.

## 6. Opponent Reactions → Responses (Mobility Ladder)

1) **Circle to outside knee line**
   - Response: crossover/scoot + keep knees/feet inside line.
   - Output check: opponent back in front within 1–2 beats.

2) **Shove-to-clear (backward+push)**
   - Response: foot pummel reinsertion first; then re-square.
   - Output check: barriers restored and opponent not past knees.

3) **Backstep / retreat (backward+pull)**
   - Response: follow with hips; upgrade to ankle/heel line true handle + redundancy.
   - Output check: deny disengage to two steps.

4) **Strip grips while circling (forward+pull behavior inside mobility)**
   - Response: reattach to leg line; do not reach with hands; keep hips square.
   - Output check: you maintain at least one connection through a full step.

5) **Fake pressure then run around**
   - Response: treat as circle first; re-square early; do not over-frame.
   - Output check: no outside knee line.

## 7. Failure Signatures → Fix
- **“He keeps getting around my knees”** → late re-square; crossover sooner; prioritize orientation over grips.
- **“My legs get shoved aside and I can’t get them back”** → reinsertion latency; foot pummel first, then anything else.
- **“He just steps away and I reset too”** → anti-exit missing; follow with hips, not hands; upgrade to true handle.
- **“I framed and he ran around”** → wrong family; mobility requires hips and legs, not early frames.
- **“I try to enter and he steps out”** → hands-down gate and thin handle; attach ankle/heel line before committing.

## 8. Interfaces (use-when tags)
- `open-guard_master-operating-system.md` — use when: running the master controller loop and switching profiles.
- `decision-model_dynamic-energy-theory.md` — use when: confirming backward+push/backward+pull vs pressure.
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: outside knee line is the primary threat.
- `retention_movement_foot-pummeling.md` — use when: shove-to-clear displaces barriers.
- `retention_movement_crossovers.md` — use when: you must re-square against circling.
- `retention_movement_scooting.md` — use when: you must follow retreats while staying squared.
- `application_cycle-break_to_immediate-counter.md` — use when: recovery windows appear; enforce immediate counter.
- `entries_distance_2-on-1-ankle-system.md` — use when: stopping reset by upgrading to ankle/heel line.

## 9. Diagram (ASCII)

~~~
MOBILITY PASSER DEFENSE LOOP

threat pattern: Barrier removal -> Angle (outside knee line) -> Reset (two steps)

REINSERT (foot pummel) -> RE-SQUARE (crossover/scoot) -> RE-CENTER (in front)
-> REATTACH (ankle/heel true handle + redundancy) -> RESTRICT EXIT (deny disengage)
-> repeat

GATES:
hip line threatened -> switch to DEFENSIVE CYCLE
hands-down required -> commit entry only after base event
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Keep Him In Front (mobility emphasis)
- **Start:** passer standing; defender seated open guard.
- **Defender wins:** prevent **outside knee line** for **20s** while keeping any contact.
- **Passer wins:** **outside knee line** then **hip line touch** or **pin**.
- **Rules:** passer must circle frequently; no prolonged forward pressure.
- **Reset:** hip line touch / pin / timer.
- **Rounds:** 8×20s, switch.

### 10.2 Shove-to-Clear Reinsertion
- **Start:** passer standing; defender seated.
- **Defender wins:** reinsert barriers and re-center; hold “in front” for **3s**.
- **Passer wins:** achieve **outside knee line** for **3s**.
- **Rules:** passer may only shove legs aside + circle (no forward drive).
- **Reset:** 3s hold by either side.
- **Rounds:** 8×20s, switch.

### 10.3 No Free Reset (mobility reset pattern)
- **Start:** range with light contact allowed.
- **Defender wins:** prevent **disengage to two steps** for **15s** while maintaining any contact.
- **Passer wins:** **disengage to two steps** with no contact.
- **Rules:** passer must attempt retreat/backstep repeatedly; defender must follow with hips and upgrade to ankle/heel line.
- **Reset:** disengage / timer.
- **Rounds:** 8×20s, switch.

### 10.4 Angle Denial Reps (outside knee line)
- **Start:** passer begins already near outside knee line (advantaged angle), not pinned.
- **Defender wins:** re-square and keep passer in front for **3s**.
- **Passer wins:** **hip line touch** or **pin**.
- **Rules:** defender must prioritize crossover/scoot; no committed entries until squared.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 10 reps each, switch.

### 10.5 Attach-and-Hold (true handle under circling)
- **Start:** defender begins with one ankle/heel connection.
- **Defender wins:** maintain the connection through one full passer step and prevent **disengage to two steps** for **15s**.
- **Passer wins:** strips contact then disengages to two steps.
- **Rules:** passer’s goal is strip + retreat; defender must add redundancy and follow with hips.
- **Reset:** timer / disengage.
- **Rounds:** 8×20s, switch.