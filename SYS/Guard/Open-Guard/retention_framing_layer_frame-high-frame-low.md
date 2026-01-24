PATH: SYS/Guard/Open-Guard/retention_framing_layer_frame-high-frame-low.md

# Retention Framing Layer — High Frame / Low Frame (Structure Stack)

## 1. Purpose
A framing system that protects you when mobility alone is insufficient (typically under forward+push pressure).

Rule: **use a high frame to protect posture and a low frame to protect hip line**.  
The pair buys time to turn-to-side, shrimp, and reinsert barriers.

## 2. Inputs / Preconditions
- You can detect pressure escalation (level element activating).
- You can turn-to-side and shrimp once structure is established.
- You can reinsert barriers after creating space.

## 3. Outputs / Success Criteria
- Pressure is absorbed without flattening (no pin consolidation).
- Hip line threat is prevented or reduced enough to begin a defensive cycle.
- You produce a cycle break (in front + barriers + orientation).
- You counter within 2 seconds after cycle break (no stop-pass-stop).

## 4. Core Model / Engine

### 4.1 Frame Stack Definitions
- **High frame:** blocks head/shoulder line from collapsing posture (prevents level dominance).
- **Low frame:** blocks hip line access (prevents penetration).
- **Stack:** high + low together, coordinated with turning to the side.

### 4.2 Timing Rule (frames are early tools)
Frames must begin at **Level threat**, not at **Penetration**.
If you wait until hip line is threatened, frames become a salvage operation.

### 4.3 Domain Progression Chain Hooks
Frames primarily deny:
- **Level** (posture compression), which prevents
- **Penetration** (hip line access), which prevents
- **Pin** (consolidation).

## 5. Gates (override rules)

### 5.1 Hip Line Gate
Hip line threatened = defensive cycle until cycle break.

**Default action:** establish frame stack → turn-to-side → shrimp/recover barriers → re-square.

### 5.2 Orientation Rule
Feet or knees face opponent. Under pressure, orientation is regained via turn-to-side + barrier reinsertion.

**Default action:** do not frame flat; frame while turning to the side so you can regain facing.

### 5.3 Hands-Down Gate (commitment)
No committed entries/rotations under stable base or active pressure.

**Default action:** survive and re-center first; counter only after cycle break.

## 6. Opponent Reactions → Responses (Frame Stack Use Cases)

1) **Shoulders drop / chest compresses (level threat)**
   - Response: high frame engages first; low frame protects hip line; turn-to-side.

2) **Deep step toward hips (penetration threat)**
   - Response: low frame priority; turn-to-side immediately; shrimp to rebuild barrier line.

3) **Circle under pressure (angle + level combined)**
   - Response: maintain frame stack; re-square when safe; do not abandon low frame.

4) **Flattening attempt (pin consolidation)**
   - Response: prevent flat shoulders; wedge with high frame; maintain low frame while hip escaping.

## 7. Failure Signatures → Fix
- **Framing too late** → start at level threat; don’t wait for hip line.
- **Framing flat on back** → turn-to-side while framing; flat framing loses mobility and facing.
- **Only high frame (hip line exposed)** → add low frame; hip line is the pass completion gate.
- **Only low frame (posture collapses)** → add high frame; level dominance precedes penetration.
- **Frames hold but nothing changes** → use frames to create space, then shrimp and reinsert barriers; aim for cycle break.

## 8. Interfaces (use-when tags)
- `application_pressure-passer_defense-ladder.md` — use when: identifying level and timing frames at L2/L4.
- `decision-model_dynamic-energy-theory.md` — use when: forward+push indicates structure is required.
- `retention_movement_shrimp.md` — use when: using space created by frames to reinsert knee/hip space.
- `retention_movement_reverse-shrimp.md` — use when: backing hips away to realign barriers after pressure.
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: framing must preserve/regain facing.
- `application_cycle-break_to_immediate-counter.md` — use when: enforcing counter start after recovery.

## 9. Diagram

~~~
FRAME STACK (Structure Layer)

HIGH FRAME -> protects posture / denies LEVEL
LOW FRAME  -> protects hip line / denies PENETRATION

stack = HIGH + LOW + TURN-TO-SIDE
-> create space -> SHRIMP -> REINSERT BARRIERS -> CYCLE BREAK -> COUNTER
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Level Threat Frame Timing
- **Start:** passer begins with shoulders low and hands on legs (pressure initiating).
- **Defender wins:** establish high+low frames and turn-to-side, then re-center for **3s**.
- **Passer wins:** **hip line touch** or **pin**.
- **Rules:** defender must frame immediately; no waiting for penetration; no committed entries.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 10 reps each, switch.

### 10.2 Penetration Salvage (late stage)
- **Start:** passer begins near hip line (late stage), not pinned.
- **Defender wins:** establish low frame priority, turn-to-side, shrimp to rebuild barriers, then cycle break **3s**.
- **Passer wins:** **pin** or flattened shoulders **3s**.
- **Rules:** defender must use low frame + turn first; bridging-only solutions not allowed.
- **Reset:** 3s hold / pin.
- **Rounds:** 10 reps each, switch.

### 10.3 Anti-Flattening (pin denial)
- **Start:** passer begins chest-to-chest but defender is on side (not flat).
- **Defender wins:** prevent flattening and re-guard/reinsert legs; hold **3s**.
- **Passer wins:** flatten shoulders and hold **pin** **3s**.
- **Rules:** defender must maintain high frame while hip escaping; low frame stays on hip line.
- **Reset:** 3s hold by either side.
- **Rounds:** 10 reps each, switch.