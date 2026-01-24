PATH: SYS/Guard/Open-Guard/retention_movement_crossovers.md

# Retention Movement — Crossovers (Hip Re-Square)

## 1. Purpose
A retention movement system for **re-squaring the hips** when the passer circles to win angle.

Crossovers are the primary tool to deny:
- **outside knee line**, and therefore
- downstream penetration and pin.

## 2. Inputs / Preconditions
- You can detect angle formation early (outside knee line beginning).
- You can move hips laterally without losing all barriers.
- You can reinsert barriers immediately after re-squaring.

## 3. Outputs / Success Criteria
- Opponent returns to **in front** within 1–2 beats.
- Outside knee line is denied or immediately corrected.
- Feet or knees remain facing (orientation invariant).
- You can reattach a true handle if the passer attempts to reset.

## 4. Core Model / Engine

### 4.1 What Crossovers Do
- Move hips to re-align your knee line to the opponent’s center.
- Convert a losing angle into a squared engagement.
- Preserve orientation so the movement layer can reinsert barriers.

### 4.2 Triggers (when to crossover)
Crossover is triggered by any of:
- opponent circling around your feet,
- your hips no longer squared (knees not facing),
- outside knee line forming (their torso line past your knee line),
- you feel “runaround speed” increasing.

### 4.3 Domain Progression Chain Hooks
Crossovers primarily deny:
- **Angle** (outside knee line).
Angle is the pivot element that converts contact into penetration.

## 5. Gates (override rules)

### 5.1 Orientation Rule (primary)
Feet or knees face opponent.

**Default action:** crossover immediately when outside knee line begins forming.

### 5.2 Hip Line Gate
If hip line is threatened, crossover alone is not enough; switch to defensive cycle.

**Default action:** frames high/low → turn-to-side → shrimp → rebuild → re-square.

### 5.3 Hands-Down Gate (commitment)
Crossovers are for re-centering, not for committing to entries under stable base.

**Default action:** re-center first; commit only after base event.

## 6. Opponent Reactions → Responses

1) **Circle acceleration (mobility passer runaround)**
   - Response: crossover earlier; keep knee line aimed; reinsert barriers immediately.

2) **Circle + shove-to-clear**
   - Response: crossover to square → foot pummel reinsertion.

3) **Circle then retreat/backstep**
   - Response: follow with hips while staying squared; upgrade to ankle/heel line true handle.

4) **Circle under pressure (angle + level)**
   - Response: do not abandon structure; frame stack first if pressure compresses, then re-square when safe.

## 7. Failure Signatures → Fix
- **I crossover but still get passed** → you crossed over late; trigger earlier on outside knee line.
- **I crossover and my legs disappear** → reinsertion missing; add foot pummel immediately after re-square.
- **I chase with hands instead of hips** → hips must travel; hands reinforce after re-square.
- **I crossover into pressure** → misread; if shoulders are dropping, frame stack first.

## 8. Interfaces (use-when tags)
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: angle/orientation is threatened.
- `application_mobility-passer_defense-loop.md` — use when: circling is primary threat.
- `retention_movement_foot-pummeling.md` — use when: crossover must be followed by barrier reinsertion.
- `retention_movement_scooting.md` — use when: following retreats while staying squared is required.
- `retention_framing_layer_frame-high-frame-low.md` — use when: circling occurs under compression (level threat).
- `decision-model_dynamic-energy-theory.md` — use when: distinguishing circle vs pressure changes the response family.

## 9. Diagram

~~~
CROSSOVERS = HIP RE-SQUARE TOOL

trigger: outside knee line forming / hips not facing
action: move hips to re-square -> knee line faces opponent -> reinsert barriers

denies: ANGLE (outside knee line)
follow-up: FOOT PUMMELING to restore barriers
if hip line threatened -> DEFENSIVE CYCLE
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Outside Knee Line Denial (crossover timing)
- **Start:** passer standing; defender seated open guard.
- **Defender wins:** prevent **outside knee line** for **20s**.
- **Passer wins:** **outside knee line** then **hip line touch** or **pin**.
- **Rules:** passer must circle continuously; defender may only use crossover-style hip re-square (no committed entries).
- **Reset:** hip line touch / pin / timer.
- **Rounds:** 8×20s, switch.

### 10.2 Angle Start Re-Square (disadvantaged reps)
- **Start:** passer begins already near outside knee line (advantaged angle), not pinned.
- **Defender wins:** re-square and keep passer in front for **3s**.
- **Passer wins:** **hip line touch** or **pin**.
- **Rules:** defender must crossover immediately; then reinsert barriers (no entry attempts).
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 10 reps each, switch.

### 10.3 Crossover + Reinsertion Combo
- **Start:** passer circles then performs a shove-to-clear once per round.
- **Defender wins:** crossover to re-square, then foot pummel to reinsert; hold “in front” for **3s**.
- **Passer wins:** **outside knee line** for **3s** or **hip line touch**.
- **Rules:** defender must sequence: re-square first, then reinsertion.
- **Reset:** 3s hold / hip line touch.
- **Rounds:** 8×20s, switch.