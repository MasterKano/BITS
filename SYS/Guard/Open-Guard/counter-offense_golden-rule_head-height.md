PATH: SYS/Guard/Open-Guard/counter-offense_golden-rule_head-height.md

# Counter-Offense — Golden Rule (Head Height)

## 1. Purpose
A counter-offense selector that converts a defensive win (re-center / cycle break) into immediate threat.

Golden Rule: **head height determines the safest and fastest counter lane**.
- **Head high** → leg lane (attack legs / secure leg line)
- **Head low** → go-behind / upper-body lane (take the space behind the head/shoulders)

This prevents “counter hesitation” and reduces stop-pass-stop behavior.

## 2. Inputs / Preconditions
- You have achieved at least one:
  - re-center (opponent in front), or
  - cycle break (after defensive cycle).
- You can read head height (high vs low) relative to your hip line.
- You can maintain orientation (feet or knees facing) while initiating the counter.

## 3. Outputs / Success Criteria
Within 2 seconds of cycle break or clear re-center, you initiate a counter that produces:
- a **true handle** on the leg line (head high), or
- a **go-behind entry** / behind-the-head position (head low), or
- forces a base event (post/widen/forced step) that opens committed follow-ups.

Failure = you recover and pause, allowing reset or re-entry into the pass chain.

## 4. Core Model / Engine

### 4.1 Golden Rule (binary selector)
- **Head high:** choose **leg lane**
  - attach ankle/heel line (true handle)
  - keep them in front while threatening the legs
- **Head low:** choose **go-behind lane**
  - occupy space behind head/shoulders
  - convert head position into angle denial and rear access

### 4.2 Counter Window (timing)
Counter must begin **immediately** after:
- **Cycle Break**, or
- **re-center** that clearly denies outside knee line and hip line threat.

Treat “pause” as granting the passer a free reset.

### 4.3 Context routing (head height × base state)
Use this to avoid lane mistakes:

| Context | Primary lane | Notes |
|---|---|---|
| Standing + head high | Leg lane | easiest to attach ankle/heel; stop retreat |
| Standing + head low | Go-behind lane | punish posture; do not chase if it breaks orientation |
| Kneeling + head high | Leg lane | leg line is close; base-break often follows |
| Kneeling + head low | Go-behind lane | strong if you are already squared; otherwise re-center first |

## 5. Gates (override rules)

### 5.1 Hip Line Gate
If hip line is threatened, you are still defending; counter is delayed until cycle break.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square.

### 5.2 Hands-Down Gate (for committed rotations/entries)
No committed entry/rotation under stable base.

**Default action:** base-break until post/widen/forced step occurs, then commit.

### 5.3 Orientation Rule
Feet or knees must face opponent.

**Default action:** re-square hips before initiating counter if orientation is lost.

## 6. Opponent Reactions → Responses (Counter Loop)
The passer’s immediate reactions to your counter attempt:

1) **Retreat / backstep to reset**
   - Head high response: maintain ankle/heel line; follow with hips; add redundancy.
   - Head low response: follow behind the head/shoulders; keep them in front (don’t chase hands).

2) **Drive forward to re-enter pressure**
   - Head high response: keep leg line; use barriers to prevent level change; re-center.
   - Head low response: disengage from chase if it breaks orientation; return to barriers then reselect lane.

3) **Strip grips while circling**
   - Head high response: upgrade to true handle (ankle/heel line); keep knees/feet between bodies.
   - Head low response: occupy space and deny outside knee line; re-center.

4) **Drop head height (high → low) mid-sequence**
   - Switch lanes if stable; if switching breaks orientation, stay leg lane and re-center first.

## 7. Failure Signatures → Fix
- **Recovered guard, then nothing happened** → counter window violated; enforce “2-second start” rule.
- **Went go-behind and lost facing** → lane selected without orientation; re-square first, then punish.
- **Chased legs under pressure and got flattened** → hip line gate ignored; defend until cycle break.
- **Kept losing contact when he backed up** → thin handle; upgrade to ankle/heel line + redundancy.
- **Always stuck between lanes** → commit to one lane per read; re-read only on clear head height change.

## 8. Interfaces (use-when tags)
- `open-guard_master-operating-system.md` — use when: enforcing cycle break → counter as the master loop.
- `application_cycle-break_to_immediate-counter.md` — use when: training timing and non-negotiable immediacy.
- `decision-model_three-laws_kneeling-standing-head.md` — use when: kneeling/standing context refines lane choice.
- `decision-model_dynamic-energy-theory.md` — use when: push/pull + forward/back changes counter stability.
- `entries_distance_2-on-1-ankle-system.md` — use when: head high and distance exists; attach ankle/heel line early.
- `entries_distance_shin-to-shin_connector.md` — use when: mid-range leg lane entry connection is required.
- `entries_kneeling_single-leg-entry.md` — use when: kneeling exposes a reachable leg under compromised posture.
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: lane switching threatens orientation.

## 9. Diagram (ASCII)

~~~
GOLDEN RULE (Counter-Offense) = HEAD HEIGHT SELECTOR

CYCLE BREAK / RECENTER -> (within 2s) COUNTER START

HEAD HIGH -> LEG LANE
  - attach ankle/heel line (true handle)
  - follow retreats; keep in front; add redundancy

HEAD LOW  -> GO-BEHIND / UPPER LANE
  - occupy space behind head/shoulders
  - deny outside knee line; re-center

CONTEXT ROUTE:
standing -> reset threat high (follow required)
kneeling -> pressure threat high (structure may be required)

GATES OVERRIDE:
HIP LINE -> DEFENSIVE CYCLE
NO HANDS-DOWN -> NO COMMITTED ENTRY/ROTATION
ORIENTATION -> INVARIANT
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Two-Second Counter Start
- **Start:** passer mid-pass attempt; defender must recover to cycle break.
- **Defender wins:** achieve cycle break then begin a counter within **2s** (leg-line true handle or go-behind entry).
- **Passer wins:** **pin** or **disengage to two steps** after defender recovers.
- **Rules:** if defender pauses after recovery, rep is a loss.
- **Reset:** counter start / pin / disengage.
- **Rounds:** 10 reps each, switch.

### 10.2 Head-High Leg Lane
- **Start:** passer stays upright (head high); defender seated open guard.
- **Defender wins:** secure ankle/heel line (true handle) and keep passer in front for **3s**.
- **Passer wins:** **outside knee line** then **hip line touch** or **pin**.
- **Rules:** passer may retreat/backstep; defender must follow and keep handle.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 8×20s, switch.

### 10.3 Head-Low Go-Behind Lane
- **Start:** passer must keep head low when engaging (posture forward); defender open guard.
- **Defender wins:** initiate go-behind lane and keep passer in front / behind head line for **3s**.
- **Passer wins:** **pin** or **hip line touch**.
- **Rules:** defender may abandon go-behind if it breaks orientation; must re-center then retry.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 8×20s, switch.

### 10.4 Lane Switching (high ↔ low)
- **Start:** passer alternates posture naturally; defender seated open guard.
- **Defender wins:** choose the correct lane and start the counter within **2s** of the head height change; then hold advantage **3s**.
- **Passer wins:** **disengage to two steps** or **pin**.
- **Rules:** defender must not chase if it breaks orientation; re-square first, then reselect lane.
- **Reset:** 3s hold / disengage / pin.
- **Rounds:** 8×20s, switch.