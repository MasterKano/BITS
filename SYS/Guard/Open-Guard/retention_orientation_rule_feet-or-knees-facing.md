PATH: SYS/Guard/Open-Guard/retention_orientation_rule_feet-or-knees-facing.md

# Retention Orientation Rule — Feet or Knees Facing (Invariant)

## 1. Purpose
A single invariant that governs Open Guard retention:

**At least one of your feet or your knees must face the opponent at all times.**

If neither faces the opponent (“double loss”), the opponent is free to:
- win outside knee line,
- threaten hip line,
- enter the penetration phase rapidly.

This rule reduces late defence by forcing early re-squaring behavior.

## 2. Inputs / Preconditions
- You can identify when the opponent is winning angle (outside knee line forming).
- You can re-square hips using movement layer options (crossover/scoot/pendulum).
- You can reinsert barriers when legs are displaced.

## 3. Outputs / Success Criteria
- The opponent cannot establish or hold outside knee line.
- Your hips re-square within 1–2 beats when angle forms.
- Your barriers reappear between bodies after shove-to-clear.
- You can transition to defensive cycle immediately if hip line is threatened.

## 4. Core Model / Engine

### 4.1 Orientation States
- **Feet facing:** your feet form the forward barrier line (distance/angle control).
- **Knees facing:** your knees/hips are squared and can reinsert feet or frames quickly.
- **Double loss (failure):** neither feet nor knees face opponent.

### 4.2 The Replacement Rule (how to keep the invariant)
If one facing tool is displaced, the other replaces it immediately:

- feet displaced → knees must face (re-square) so feet can be reinserted  
- knees turned away → feet must face (re-barrier) to prevent angle runaround

### 4.3 Domain Progression Chain Hooks
Orientation loss primarily enables:
- **Angle** (outside knee line) → which enables
- **Penetration** (hip line access) → which enables
- **Pin**.

So you treat orientation as an early-warning system.

## 5. Gates (override rules)

### 5.1 Orientation Rule (primary)
This is the invariant: feet or knees facing at all times.

**Default action:** re-square hips immediately when outside knee line is forming.

### 5.2 Hip Line Gate
If hip line is threatened, you are in defensive cycle until cycle break.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square.

### 5.3 Hands-Down Gate (commitment)
No committed entries/rotations under stable base.

**Default action:** maintain orientation first; base-break or re-center before committing.

## 6. Opponent Reactions → Responses (Orientation Ladder)

1) **Circle to outside knee line**
   - Response: crossover/scoot to re-square; keep knees facing.
   - Output check: opponent back in front within 1–2 beats.

2) **Shove-to-clear (legs displaced)**
   - Response: knees face immediately (re-square) → foot pummel reinsertion.
   - Output check: barriers reappear between bodies.

3) **Pressure compress (shoulders low)**
   - Response: keep knees facing via turn-to-side; frames protect while you regain feet position.
   - Output check: no flattening, no deep step to hip line.

4) **Backstep/retreat**
   - Response: follow with hips while keeping knees facing; reattach ankle line if possible.
   - Output check: no disengage to two steps.

## 7. Failure Signatures → Fix
- **“He ran around my legs”** → knees weren’t facing; re-square sooner; hips must travel.
- **“My legs got shoved aside and I stayed square but still got passed”** → you were square but barriers didn’t reinsert; foot pummel sooner.
- **“I turned away to frame and lost angle”** → frames without facing; turn-to-side while keeping knees orientation, then reinsert legs.
- **“I got surprised by penetration”** → ignored double loss; treat it as an alarm and re-square immediately.

## 8. Interfaces (use-when tags)
- `retention_movement_crossovers.md` — use when: outside knee line is forming and hips must re-square.
- `retention_movement_scooting.md` — use when: you must follow circling/retreat while staying squared.
- `retention_movement_pendulum.md` — use when: you need angle/distance recovery without conceding hip line.
- `retention_movement_foot-pummeling.md` — use when: legs are shucked and barriers must be reinserted.
- `retention_framing_layer_frame-high-frame-low.md` — use when: pressure compresses and you must protect while reorienting.
- `open-guard_master-operating-system.md` — use when: orientation loss forces a phase switch or rerouting.
- `retention_model_six-elements-of-passing.md` — use when: mapping orientation loss to angle/penetration elements.

## 9. Diagram

~~~
ORIENTATION INVARIANT

Rule: at least one of {FEET, KNEES} faces opponent at all times

If FEET are displaced -> KNEES must face (re-square) -> reinsert FEET
If KNEES turn away     -> FEET must face (barrier)  -> prevent angle

Failure = DOUBLE LOSS (neither faces) -> Angle -> Penetration -> Pin
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Outside Knee Line Denial
- **Start:** passer standing; defender seated open guard.
- **Defender wins:** prevent **outside knee line** for **20s**.
- **Passer wins:** achieve **outside knee line** then **hip line touch** or **pin**.
- **Rules:** defender may not commit entries; only goal is orientation maintenance and re-square.
- **Reset:** hip line touch / pin / timer.
- **Rounds:** 8×20s, switch.

### 10.2 Shove-to-Clear Reinsertion (feet displaced)
- **Start:** passer standing; defender seated.
- **Defender wins:** after shove, re-square and reinsert barriers, then hold “in front” for **3s**.
- **Passer wins:** **outside knee line** for **3s** or **hip line touch**.
- **Rules:** passer may only shove legs aside + circle; defender must re-square first, then foot pummel.
- **Reset:** 3s hold / hip line touch.
- **Rounds:** 8×20s, switch.

### 10.3 Double-Loss Alarm Reps
- **Start:** passer begins at a slight angle (near outside knee line). Defender starts with feet and knees not facing (simulated error).
- **Defender wins:** restore feet-or-knees facing and re-center within **2 beats**, then hold **3s**.
- **Passer wins:** **hip line touch** or **pin**.
- **Rules:** defender’s only job is to fix orientation immediately; no counters until fixed.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 10 reps each, switch.