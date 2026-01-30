PATH: SYS/Guard/Open-Guard/retention_movement_scissor-roll.md

# Retention Movement — Scissor Roll (Rotational Barrier Replacement)

## 1. Purpose
A retention movement system for replacing barriers via a controlled rotation when the passer is winning angle and clearing your legs.

Scissor roll is used to:
- restore facing (feet/knees facing),
- reinsert a barrier line when one leg is beaten,
- prevent the angle → penetration cascade.

## 2. Inputs / Preconditions
- You have enough space to rotate (not fully pinned).
- You can keep at least one barrier or frame active during the roll.
- You can finish the roll with knees/feet facing (orientation restored).

## 3. Outputs / Success Criteria
- You replace a beaten barrier with a new barrier (leg returns between bodies).
- Opponent returns to in front (outside knee line denied or corrected).
- Hip line threat does not increase during the rotation.
- You can reattach (ankle/heel line) if the passer attempts to reset.

## 4. Core Model / Engine

### 4.1 What Scissor Roll Does
- Uses rotation to “swap” which leg is the primary barrier.
- Prevents the passer from running around a dead leg line.
- Rebuilds a functional barrier platform for re-centering.

### 4.2 Triggers (when to scissor roll)
Use scissor roll when:
- one leg is beaten and you cannot reinsert with foot pummeling fast enough,
- angle is forming and you need a rotational replacement rather than lateral travel,
- seated pivot (scissor sit) is insufficient.

If hip line is already threatened under heavy pressure, switch to defensive cycle tools first.

### 4.3 Domain Progression Chain Hooks
Scissor roll primarily denies:
- **Angle** and **Distance** (barrier removal), preventing penetration.

## 5. Gates (override rules)

### 5.1 Orientation Rule (primary)
Finish the roll with feet or knees facing opponent.

**Default action:** stop rotation as soon as facing is restored; re-center immediately.

### 5.2 Hip Line Gate
If hip line is threatened, rotational recovery is risky; switch to defensive cycle.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square.

### 5.3 Hands-Down Gate (commitment)
Scissor roll is recovery, not entry commitment.

**Default action:** re-center first; commit only after base event.

## 6. Opponent Reactions → Responses

1) **Circle acceleration (tries to beat the new barrier)**
   - Response: finish roll into facing, then immediate re-square and reinsertion.

2) **Shove-to-clear during rotation**
   - Response: complete rotation, then foot pummel reinsertion; do not chase hands.

3) **Retreat after you recover**
   - Response: scoot-follow; upgrade to ankle/heel line true handle to deny disengage.

4) **Pressure drop as you roll**
   - Response: abandon extended rotation; establish frame stack and turn-to-side; treat as pressure profile.

## 7. Failure Signatures → Fix
- **I roll and give up my back/angle** → rotation overshoots; stop as soon as facing returns; re-center.
- **I roll but still have no barriers** → missing reinsertion; roll must end with a barrier between bodies.
- **I roll into pressure and get pinned** → misread; pressure requires frames; do not roll under heavy compression.
- **I use scissor roll when foot pummel would work** → tool selection error; reserve roll for when reinsertion is too slow.

## 8. Interfaces (use-when tags)
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: rotation must restore facing.
- `retention_movement_foot-pummeling.md` — use when: roll finishes and requires reinsertion to stabilize.
- `retention_movement_scissor-sit.md` — use when: seated pivot is sufficient instead of rotation.
- `retention_movement_crossovers.md` — use when: lateral hip travel can re-square without rotation.
- `application_mobility-passer_defense-loop.md` — use when: circling is primary threat; roll is a recovery tool inside the loop.
- `retention_framing_layer_frame-high-frame-low.md` — use when: pressure appears and rotation is unsafe.

## 9. Diagram

~~~
SCISSOR ROLL = ROTATIONAL BARRIER REPLACEMENT

trigger: one barrier beaten + angle forming + reinsertion too slow
action: controlled rotation -> swap barrier -> finish with facing -> re-center
follow-up: stabilize with FOOT PUMMELING / reattachment

denies: Angle + Distance
if hip line threatened -> DEFENSIVE CYCLE
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Beaten-Leg Recovery (scissor roll trigger)
- **Start:** passer begins with one of defender’s legs already beaten to the outside; defender not pinned.
- **Defender wins:** scissor roll to replace barrier and keep passer in front for **3s**.
- **Passer wins:** **hip line touch** or **pin**.
- **Rules:** defender must use scissor roll as primary recovery (no standing, no committed entries).
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 10 reps each, switch.

### 10.2 Roll → Reinsertion Stabilization
- **Start:** passer circles and can shove-to-clear once per rep.
- **Defender wins:** scissor roll, then foot pummel reinsertion; hold “in front” **3s**.
- **Passer wins:** **outside knee line** **3s** or **hip line touch**.
- **Rules:** mandatory sequence: roll first, reinsertion second.
- **Reset:** 3s hold / hip line touch.
- **Rounds:** 8×20s, switch.

### 10.3 Wrong-Tool Penalty (pressure check)
- **Start:** passer begins with shoulders low (pressure initiating).
- **Defender wins:** use frames/turn/shrimp to cycle break; no scissor roll used.
- **Passer wins:** **pin** or flattened shoulders **3s**.
- **Rules:** if defender attempts scissor roll under pressure, restart rep (teaches tool selection).
- **Reset:** cycle break / pin / 3s hold.
- **Rounds:** 10 reps each, switch.