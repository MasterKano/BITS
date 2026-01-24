PATH: SYS/Guard/Open-Guard/entries_distance_partial-inversion_distance-breaker.md

# Entries (Distance) — Partial Inversion Distance Breaker (Gate-Based)

## 1. Purpose
A distance-breaking entry system that uses **partial inversion** to collapse space and access deeper connections when distance entries alone are insufficient.

Key constraint: **partial inversion is only valid under a base-compromise signal** (hands-down / forced step / widened base).  
The purpose is not “invert because you can,” but to **break distance safely** and convert into a stable connector.

## 2. Inputs / Preconditions
- You are at distance or mid-range (not already flattened).
- You can read base compromise (hands-down / forced step / widened base).
- You can preserve orientation on exit (finish facing and with barriers restored).

## 3. Outputs / Success Criteria
- Distance is broken (opponent cannot freely reset to two steps).
- You achieve a stable connector (shin-to-shin or leg-line control) without conceding hip line.
- You force a base event or exploit an existing one.
- You return to re-centered facing after the breaker, ready to continue offense or re-guard.

## 4. Core Model / Engine

### 4.1 What “Partial Inversion Distance Breaker” is
A controlled partial inversion that:
- changes your hip line relative to the opponent’s leg line,
- brings your legs back between bodies,
- collapses their space and prevents easy disengagement.

It is a **distance management tool** that becomes an entry only when the gate is satisfied.

### 4.2 Validity Condition (Hands-Down / Base Compromise Gate)
You may use partial inversion only when at least one is true:
- opponent posts hands (hands-down),
- opponent widens base visibly,
- opponent takes a forced step that breaks posture alignment.

If none are present, do not invert; use 2-on-1 ankle, shin-to-shin, crossovers/pendulum.

### 4.3 Breaker Loop (repeatable)
**CREATE/READ BASE EVENT → PARTIAL INVERT → COLLAPSE DISTANCE → CONNECTOR → RE-SQUARE**

- base event is the permission slip
- partial inversion collapses space
- connector stabilizes the position
- re-square prevents angle loss

## 5. Gates (override rules)

### 5.1 Hands-Down Gate (primary)
No inversion under stable base.

**Default action:** if stable base: use 2-on-1 ankle + off-balance to force base event.

### 5.2 Hip Line Gate
If hip line is threatened, inversion is unsafe; defend first.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square → re-enter at distance.

### 5.3 Orientation Rule
Finish with feet or knees facing opponent.

**Default action:** stop rotation as soon as facing is restored; reinsert barriers immediately.

## 6. Opponent Reactions → Responses

1) **Base recovers mid-breaker**
   - Response: abort deeper rotation; re-square and rebuild barriers; return to handle-based entries.

2) **Passer circles to chase angle during the breaker**
   - Response: finish to facing quickly; add crossover re-square; do not continue rotating.

3) **Passer retreats as you connect**
   - Response: maintain connector; scoot-follow; upgrade to ankle/heel line true handle.

4) **Passer drops into pressure after distance is broken**
   - Response: frame stack appears; treat as pressure profile; defensive cycle if hip line threatened.

## 7. Failure Signatures → Fix
- **I inverted and got smashed** → gate violated; no inversion under stable base.
- **I inverted and lost orientation** → overspin; finish facing quickly; reinsert barriers.
- **Breaker doesn’t actually break distance** → no connector; add shin-to-shin / ankle-line control immediately.
- **I use breaker when simple handle works** → tool selection; default to 2-on-1 ankle unless base event demands breaker.

## 8. Interfaces (use-when tags)
- `entries_distance_2-on-1-ankle-system.md` — use when: forcing base events and building permission for breaker.
- `entries_distance_shin-to-shin_connector.md` — use when: the primary connector after distance is collapsed.
- `decision-model_dynamic-energy-theory.md` — use when: verifying hands-down/base compromise gating for inversion.
- `retention_movement_inverted-spin.md` — use when: inversion is used defensively for angle escape (not distance breaking).
- `retention_movement_crossovers.md` — use when: re-squaring after breaker to deny outside knee line.
- `application_pressure-passer_defense-ladder.md` — use when: breaker triggers pressure; switch to structure.

## 9. Diagram

~~~
PARTIAL INVERSION DISTANCE BREAKER (Gate-Based)

stable base -> NO INVERSION
base event (hands-down / widened / forced step) -> partial invert -> collapse distance
-> CONNECTOR (shin-to-shin / leg line) -> re-square -> continue

abort rules:
base recovers / angle chase -> stop rotation -> face -> reinsert barriers
hip line threatened -> defensive cycle
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Gate Recognition (inversion permission)
- **Start:** passer standing; defender seated open guard.
- **Defender wins:** only invert after a visible base event; then connect and re-center **3s**.
- **Passer wins:** if defender inverts under stable base and is pinned within **5s**, or achieves **hip line touch**.
- **Rules:** passer alternates between stable base and occasional posts/forced steps; defender must obey the gate.
- **Reset:** 3s hold / hip line touch / pin event.
- **Rounds:** 10 reps each, switch.

### 10.2 Break Distance → Connector
- **Start:** defender begins with 2-on-1 ankle; passer attempts to keep range and stable base.
- **Defender wins:** force base event, then partial inversion to break distance and establish connector within **10s**.
- **Passer wins:** maintain stable base and disengage to two steps within **10s**.
- **Rules:** defender may not invert until base event occurs; connector must be established after inversion.
- **Reset:** connector established / timer / disengage.
- **Rounds:** 10 reps each, switch.

### 10.3 Abort and Recover
- **Start:** passer gives a brief post (gate appears) then recovers base quickly.
- **Defender wins:** begin breaker only if allowed, then abort and re-square when base returns; hold “in front” **3s**.
- **Passer wins:** **outside knee line** then **hip line touch** or **pin**.
- **Rules:** defender must demonstrate “stop rotation when permission disappears.”
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 8×20s, switch.