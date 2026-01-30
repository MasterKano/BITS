PATH: SYS/Guard/Open-Guard/retention_model_knowledge-denial.md

# Retention Model — Knowledge Denial (Requirements-First)

## 1. Purpose
A retention model that replaces “defend named passes” with:

**Deny the requirements the passer must assemble.**

If the passer cannot build the next requirement link, the pass does not happen. This model improves timing and reduces late, reactive defence.

## 2. Inputs / Preconditions
- You can re-center (keep opponent in front).
- You can reinsert barriers when displaced.
- You can maintain orientation (feet or knees facing).
- You can identify which requirement link is being built now (distance/grip/angle/level/penetration/pin).

## 3. Outputs / Success Criteria
- The passer is forced to **re-build** repeatedly (re-step/re-grip/re-square).
- You deny progress to the next requirement link.
- You avoid hip line threat; if threatened, you enter defensive cycle immediately.
- You maintain at least one connection or quickly reattach (anti-reset).

## 4. Core Model / Engine

### 4.1 Knowledge Denial Rule
You do not “solve passes.” You deny the **current requirement** and re-center.

Loop:
**READ (current link) → DENY (break it) → RECENTER → RE-READ**

### 4.2 Domain Progression Chain Table (passing requirements)
Use this to label what is happening *now*.

| Link | What you read (signal) | What you deny (action) |
|---|---|---|
| Distance | barriers removed; legs pushed aside; space collapses | reinsert barriers; knees/feet inside line; re-center |
| Grip | stable anchors on legs/hips/upper body | strip/downgrade; build your own true handle + redundancy |
| Angle | outside knee line forming; hips not squared | crossover/scoot/pendulum; enforce orientation |
| Level | shoulders drop; pressure compresses posture | frames high/low; turn-to-side early |
| Penetration | hip line threatened; legs cleared near hips | defensive cycle; shrimp to rebuild barriers; re-square |
| Pin | shoulders flatten; chest-to-chest consolidation | prevent flattening; rebuild frames; re-guard/reinsert legs |

### 4.3 Denial Priorities (fast rules)
- Deny **Angle** earlier than you think (outside knee line is the pivot link).
- Deny **Level** before **Penetration** (frames early are cheaper than late shrimping).
- Deny **Reset** by keeping at least one reliable connection (true handle when possible).

## 5. Gates (override rules)

### 5.1 Hip Line Gate
Hip line threatened = defensive cycle until cycle break.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square.

### 5.2 Hands-Down Gate
No committed rotation/entry under stable base.

**Default action:** defend and re-center first; commit only after base event.

### 5.3 Orientation Rule
Feet or knees face opponent.

**Default action:** re-square hips immediately when outside knee line is forming.

## 6. Opponent Reactions → Responses (Denial Patterns)

1) **Shove-to-clear (barrier removal)**
   - Deny: distance link.
   - Response: foot pummel reinsertion first; then re-square.

2) **Circle to outside knee line**
   - Deny: angle link.
   - Response: crossover/scoot; keep opponent in front.

3) **Drop shoulders to compress**
   - Deny: level link.
   - Response: frames high/low; turn-to-side; deny shoulder line.

4) **Step deep toward hips**
   - Deny: penetration link.
   - Response: defensive cycle; shrimp; rebuild barriers; cycle break check.

5) **Backstep/retreat after you re-center**
   - Deny: reset.
   - Response: follow with hips; upgrade to ankle/heel line true handle.

## 7. Failure Signatures → Fix
- **Late defence (always at penetration)** → you are reading too late; label the link earlier (angle/level).
- **Hand chasing** → re-square hips first; hands reinforce, not lead.
- **Barriers keep disappearing** → reinsertion latency; foot pummel first, then anything else.
- **Frames collapse under pressure** → build high/low frame earlier (at level link), not after flattening begins.
- **He resets freely** → thin/no handle; upgrade to ankle/heel line + redundancy; follow with hips.

## 8. Interfaces (use-when tags)
- `open-guard_master-operating-system.md` — use when: running the full controller loop (deny link → re-center → counter).
- `retention_model_six-elements-of-passing.md` — use when: deeper breakdown of pass-building elements is needed.
- `decision-model_dynamic-energy-theory.md` — use when: push/pull + forward/back determines which denial tool family is correct.
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: angle/outside knee line is the primary threat.
- `retention_framing_layer_frame-high-frame-low.md` — use when: denying level/pressure requires structure.
- `retention_movement_foot-pummeling.md` — use when: distance link is attacked via shucking/clearing.
- `retention_movement_crossovers.md` — use when: angle link is attacked via circling.
- `application_cycle-break_to_immediate-counter.md` — use when: enforcing conversion after defensive cycle.

## 9. Diagram

~~~
KNOWLEDGE DENIAL (Requirements-First Retention)

READ current link -> DENY it -> RECENTER -> re-read

Passing requirements chain:
Distance -> Grip -> Angle -> Level -> Penetration -> Pin

You win by preventing assembly:
- deny early links (Angle/Level) to avoid late Penetration defence
- keep orientation invariant
- if hip line threatened -> defensive cycle until cycle break
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Link Denial Rounds
- **Start:** passer standing; defender seated open guard.
- **Defender wins:** prevent **outside knee line** and **hip line touch** for **20s**.
- **Passer wins:** **outside knee line** then **hip line touch** or **pin**.
- **Rules:** defender must treat each passer attempt as “which link is this?” and deny it immediately (no stalling).
- **Reset:** hip line touch / pin / timer.
- **Rounds:** 8×20s, switch.

### 10.2 Angle-First Denial (outside knee line)
- **Start:** passer begins already near outside knee line (advantaged angle), not pinned.
- **Defender wins:** re-square and keep passer in front for **3s**.
- **Passer wins:** **hip line touch** or **pin**.
- **Rules:** defender may not commit entries until squared; priority is angle denial.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 10 reps each, switch.

### 10.3 Level Denial (frame timing)
- **Start:** passer begins with shoulders low and hands on legs (level link active).
- **Defender wins:** establish high/low frames and turn-to-side, then re-center for **3s**.
- **Passer wins:** **hip line touch** or **pin**.
- **Rules:** defender must frame immediately; no waiting for penetration.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 10 reps each, switch.

### 10.4 Reset Denial (anti-exit)
- **Start:** range with light contact allowed.
- **Defender wins:** maintain any contact for **15s** and upgrade to a true handle when possible.
- **Passer wins:** **disengage to two steps** with no contact.
- **Rules:** passer must attempt retreat/backstep repeatedly; defender must follow with hips.
- **Reset:** disengage / timer.
- **Rounds:** 8×20s, switch.