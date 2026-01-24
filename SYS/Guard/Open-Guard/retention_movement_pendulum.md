PATH: SYS/Guard/Open-Guard/retention_movement_pendulum.md

# Retention Movement — Pendulum (Angle + Distance Recovery)

## 1. Purpose
A retention movement system for recovering **angle and distance** without conceding the hip line.

Pendulum is used when:
- the passer is starting to win angle,
- your barriers are partially compromised,
- you need a rapid re-centering tool that preserves orientation.

## 2. Inputs / Preconditions
- You can create a small amount of space with hips/legs (not necessarily frames).
- You can keep at least one barrier between bodies during the movement.
- You can re-square hips and reinsert barriers immediately after the swing.

## 3. Outputs / Success Criteria
- Opponent returns in front (outside knee line denied).
- You restore a usable barrier line (feet/knees between bodies).
- You avoid hip line penetration during the movement.
- You can upgrade to a true handle if the passer attempts to reset.

## 4. Core Model / Engine

### 4.1 What Pendulum Does
- Uses a controlled hip swing to re-align your knee/foot line to the opponent’s center.
- Recovers distance while maintaining facing.
- Converts “almost angle loss” into a squared engagement without needing full frames.

### 4.2 Triggers (when to pendulum)
Use pendulum when:
- opponent is circling and you’re late for a pure crossover,
- you need to change your hip line relative to their approach line,
- you can feel the “corner” forming but hip line is not yet threatened.

If hip line is already threatened, pendulum is usually too late—switch to defensive cycle.

### 4.3 Domain Progression Chain Hooks
Pendulum primarily denies:
- **Angle** and **Distance** together,
preventing the angle → penetration cascade.

## 5. Gates (override rules)

### 5.1 Orientation Rule (primary)
Feet or knees must face opponent.

**Default action:** pendulum only while maintaining facing; if facing breaks, re-square first.

### 5.2 Hip Line Gate
Hip line threatened = pendulum is no longer the tool; defensive cycle is required.

**Default action:** frames high/low → turn-to-side → shrimp → rebuild → re-square.

### 5.3 Hands-Down Gate (commitment)
Pendulum is recovery, not entry commitment.

**Default action:** re-center first; commit only after base event.

## 6. Opponent Reactions → Responses

1) **Circle + step deep**
   - Response: pendulum early to re-center; if deep step threatens hip line, switch to defensive cycle.

2) **Shove-to-clear during swing**
   - Response: complete re-square, then immediate foot pummel reinsertion.

3) **Retreat after you re-center**
   - Response: follow with hips; upgrade to ankle/heel line true handle.

4) **Pressure drop mid-exchange**
   - Response: frame stack appears; turn-to-side; convert pendulum attempt into defensive cycle.

## 7. Failure Signatures → Fix
- **Pendulum feels like I “give my side”** → facing wasn’t preserved; pendulum must keep knees/feet pointed at opponent.
- **I pendulum and still lose outside knee line** → triggered too late; use it earlier or crossover sooner.
- **I pendulum and get smashed** → misread pressure; if shoulders drop, frame first.
- **I pendulum but my barriers are gone after** → missing reinsertion; foot pummel immediately after re-square.

## 8. Interfaces (use-when tags)
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: pendulum must preserve facing.
- `retention_movement_crossovers.md` — use when: a direct hip re-square is available earlier.
- `retention_movement_foot-pummeling.md` — use when: pendulum recovery must be followed by barrier reinsertion.
- `application_mobility-passer_defense-loop.md` — use when: circling and resets are the main threats.
- `retention_framing_layer_frame-high-frame-low.md` — use when: pressure drops and structure becomes required.
- `decision-model_dynamic-energy-theory.md` — use when: distinguishing circle vs pressure changes the response family.

## 9. Diagram

~~~
PENDULUM = ANGLE + DISTANCE RECOVERY

trigger: corner forming (late for crossover) but hip line not yet threatened
action: controlled hip swing while facing -> re-center -> re-square -> reinsert barriers

denies: Angle + Distance
follow-up: FOOT PUMMELING (reinsertion) or TRUE HANDLE upgrade
if hip line threatened -> DEFENSIVE CYCLE
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Pendulum Timing (late angle recovery)
- **Start:** passer begins near outside knee line (slight advantage), not pinned.
- **Defender wins:** pendulum to re-center and hold opponent in front for **3s**.
- **Passer wins:** achieve **hip line touch** or **pin**.
- **Rules:** defender must use pendulum as the primary recovery; no committed entries until squared.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 10 reps each, switch.

### 10.2 Pendulum + Reinsertion Combo
- **Start:** passer circles and performs a shove-to-clear once per round.
- **Defender wins:** pendulum to re-center, then foot pummel reinsertion; hold “in front” for **3s**.
- **Passer wins:** **outside knee line** for **3s** or **hip line touch**.
- **Rules:** sequence is mandatory: pendulum/re-square first, reinsertion second.
- **Reset:** 3s hold / hip line touch.
- **Rounds:** 8×20s, switch.

### 10.3 Pressure Switch (pendulum to defensive cycle)
- **Start:** passer begins circling, but is allowed to drop shoulders to pressure mid-round.
- **Defender wins:** use pendulum while mobility, then switch to frame stack/defensive cycle when pressure appears; return to cycle break.
- **Passer wins:** **pin** or flattened shoulders **3s**.
- **Rules:** defender must demonstrate correct tool family switching (mobility → structure).
- **Reset:** cycle break achieved / pin / 3s hold.
- **Rounds:** 8×20s, switch.