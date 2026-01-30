PATH: SYS/Guard/Open-Guard/retention_movement_foot-pummeling.md

# Retention Movement — Foot Pummeling (Barrier Reinsertion)

## 1. Purpose
A retention movement system for rebuilding barriers when the passer shucks, shoves, or clears your legs.

Foot pummeling is not “kicking.” It is **reinsertion of inside position** so you can:
- deny distance/barrier removal,
- deny outside knee line progression,
- prevent hip line penetration.

## 2. Inputs / Preconditions
- You can keep knees/hips mobile enough to re-square.
- You can maintain at least one contact point (hand or foot) while reinserting.
- You can switch to structural framing if pressure escalates.

## 3. Outputs / Success Criteria
- Your legs return to the inside line (barriers between bodies).
- Opponent stays in front (outside knee line denied).
- You can upgrade to true handle (ankle/heel line) after reinsertion.
- If pressure escalates, you enter defensive cycle without delay.

## 4. Core Model / Engine

### 4.1 What Foot Pummeling Actually Does
- Reclaims inside position of the legs.
- Restores “knee line barrier” that blocks the passer’s step path.
- Creates a platform for re-centering and attachment.

### 4.2 Triggers (when to pummel)
Foot pummel is triggered by any of:
- legs shoved aside (shove-to-clear),
- passer steps wide to run around,
- your feet are outside the opponent’s hips (barrier removed),
- you feel “empty space” between your knee line and their entry line.

### 4.3 Domain Progression Chain Hooks
Foot pummeling primarily denies:
- **Distance** (barrier removal) and
- **Angle** (outside knee line),
which prevents penetration.

## 5. Gates (override rules)

### 5.1 Orientation Rule
Feet or knees facing is invariant; foot pummeling is performed while keeping hips square.

**Default action:** re-square hips first if outside knee line is forming, then pummel.

### 5.2 Hip Line Gate
If hip line is threatened, foot pummeling alone is insufficient; switch to defensive cycle.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square.

### 5.3 Hands-Down Gate (commitment)
Foot pummeling is reinsertion, not entry commitment. Do not “go under” under stable base.

**Default action:** reinsert and re-center first; commit only after base event.

## 6. Opponent Reactions → Responses

1) **Shove-to-clear + circle**
   - Response: immediate pummel reinsertion → re-square → re-center.

2) **Pin the legs down (heavy leg)**
   - Response: pummel in small increments; use hip movement to create insertion space; reinsert one barrier at a time.

3) **Retreat after clearing**
   - Response: follow with hips while maintaining any contact; reattach ankle/heel line after reinsertion.

4) **Pressure drop during reinsertion**
   - Response: frame stack appears; turn-to-side; convert to defensive cycle.

## 7. Failure Signatures → Fix
- **I pummel but he still runs around** → hips not squared; re-square first, then pummel.
- **My feet are “outside” and useless** → you’re pummeling too late; trigger earlier on shove-to-clear.
- **I keep losing the same leg** → lack of redundancy; reinsert one barrier then reinforce with the other leg/hand.
- **I pummel into pressure and get flattened** → misread; pressure gate; frame and turn first.

## 8. Interfaces (use-when tags)
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: reinsertion must preserve facing.
- `retention_movement_crossovers.md` — use when: circling creates outside knee line; re-square before reinsertion.
- `application_mobility-passer_defense-loop.md` — use when: shove-to-clear and circling are primary threats.
- `decision-model_dynamic-energy-theory.md` — use when: backward+push behavior triggers reinsertion.
- `retention_framing_layer_frame-high-frame-low.md` — use when: reinsertion is threatened by pressure (level/penetration).
- `entries_distance_2-on-1-ankle-system.md` — use when: reinsertion creates distance window for ankle/heel attachment.

## 9. Diagram

~~~
FOOT PUMMELING = BARRIER REINSERTION

trigger: legs shoved/cleared -> "empty inside line"
action: re-square hips -> reinsert one barrier -> reinforce -> reinsert second -> re-center

denies: Distance (barrier removal) + Angle (outside knee line)
if hip line threatened -> switch to DEFENSIVE CYCLE
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Shove-to-Clear Reinsertion
- **Start:** passer standing; defender seated; passer begins by shoving legs aside.
- **Defender wins:** reinsert barriers and re-center; hold “in front” for **3s**.
- **Passer wins:** **outside knee line** for **3s** or **hip line touch**.
- **Rules:** passer may only shove legs aside + circle (no forward pressure).
- **Reset:** 3s hold / hip line touch.
- **Rounds:** 8×20s, switch.

### 10.2 Heavy Leg Pin (incremental reinsertion)
- **Start:** passer pins one of defender’s legs down with shin/weight (no full pin).
- **Defender wins:** free the pinned leg and reinsert barriers; hold **3s** in front.
- **Passer wins:** achieve **outside knee line** then **hip line touch**.
- **Rules:** defender must reinsert one barrier at a time; no committed entries.
- **Reset:** 3s hold / hip line touch.
- **Rounds:** 10 reps each, switch.

### 10.3 Reinsertion → True Handle Upgrade
- **Start:** passer clears legs once; defender must recover.
- **Defender wins:** reinsert barriers then secure ankle/heel line (true handle) within **5s**.
- **Passer wins:** clears again and achieves **disengage to two steps**.
- **Rules:** defender must re-square before reaching; ankle/heel line is the target.
- **Reset:** true handle / disengage.
- **Rounds:** 10 reps each, switch.