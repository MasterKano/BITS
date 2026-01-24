PATH: SYS/Guard/Open-Guard/decision-model_dynamic-energy-theory.md

# Decision Model — Dynamic Energy Theory (Open Guard)

## 1. Purpose
A decision model that selects the correct response family in Open Guard based on the opponent’s committed effort.

Goal: prevent wrong-family decisions (e.g., framing vs mobility, spinning under stable base, accepting resets) by mapping opponent behavior to a small set of executable responses.

## 2. Inputs / Preconditions
- You can read opponent intent from movement direction + force.
- You can maintain or restore **orientation** (feet or knees facing).
- You can establish at least light contact and upgrade to a **true handle** when required.

## 3. Outputs / Success Criteria
Correct selection produces at least one observable output within 5–10 seconds:
- **Re-center:** opponent returns in front (angle denied).
- **Force base event:** post/widen/forced step (hands-down gate earned).
- **Prevent reset:** opponent cannot disengage to two clean steps.
- **Avoid hip line threat:** no penetration to hip line; if threatened, you enter defensive cycle immediately.

If none occur, assume misread quadrant, thin handle, or gate violation.

## 4. Core Model / Engine

### 4.1 Quadrant Read
Dynamic Energy = 2-axis read:
- **Push vs Pull**
- **Forward vs Backward**

Definitions:
- **Push:** compress/drive/shove barriers; builds level and penetration.
- **Pull:** strip/withdraw/backstep; attempts to reset or remove attachment.
- **Forward:** advancing into the pass chain.
- **Backward:** exiting engagement to reset distance/safety.

### 4.2 Domain Progression Chain Hooks (how the quadrant maps to the chain)
Quadrants are not “styles”; they are **which chain link is being attacked next**:

- **Forward+Push:** threatens **Level → Penetration → Pin**
- **Backward+Pull:** threatens **Reset/Disengage** (breaks your CONNECT before you can DENY)
- **Backward+Push:** threatens **Distance/Barrier removal** (shuck legs) then reset
- **Forward+Pull:** threatens **Grip/Angle** while still advancing

Use this to choose denial actions quickly (deny the current link, then re-center).

### 4.3 Default Response Families (module selection)
- **Mobility retention:** re-square + re-center (pummel/crossover/pendulum/scoot)
- **Structural defense:** frames + turn-to-side + shrimp (defensive cycle)
- **Base-break pursuit:** off-balance until hands-down gate is earned
- **Anti-exit governance:** follow + reattach; containment if already entangled

## 5. Gates (override rules)

### 5.1 Hip Line Gate (phase switch)
If hip line is threatened: you are in **DEFENSIVE CYCLE** until cycle break.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square.

### 5.2 Hands-Down Gate (entry validity)
No committed entries/rotations/spin-unders under stable base.

**Default action:** off-balance until post/widen/forced step occurs → then commit.

### 5.3 Orientation Rule (integrity)
Feet or knees must face opponent continuously.

**Default action:** re-square hips + reinsert barriers before attempting upgrades.

## 6. Opponent Reactions → Responses (Quadrant Playbook)

### 6.1 Forward + Push (pressure build)
**Read:** advancing drive/compression; posture lowering; shoulder line approaching your hips.  
**Deny:** level/penetration.  
**Response family:** structure early; do not wait for full penetration.

- frames high/low as needed
- turn-to-side before shrimping
- reinsert barriers as soon as space exists
- once cycle break achieved: counter immediately (no pause)

### 6.2 Backward + Pull (reset / backstep / flee)
**Read:** retreating while stripping contact; backstep patterns; disengage intent.  
**Deny:** reset.  
**Response family:** anti-exit governance (follow + true handle).

- immediately follow the retreat (hips travel, not hands)
- upgrade to ankle/heel line control (true handle)
- add redundancy (hand+foot) so “two steps” is slow
- if already entangled: switch to containment logic (do not chase)

### 6.3 Backward + Push (shove-to-clear then circle away)
**Read:** shove legs aside to create empty inside line; circle/run.  
**Deny:** barrier removal then reset.  
**Response family:** reinsertion + mobility.

- immediate foot pummel / barrier reinsertion
- crossover/scoot to keep opponent in front
- attach ankle line to prevent the next step-out

### 6.4 Forward + Pull (strip/bait while advancing)
**Read:** stripping grips while still stepping in; pulling your connections off-line.  
**Deny:** grip/angle.  
**Response family:** reattach leg line + re-square.

- treat strip as “reattach now,” not “reach now”
- prioritize ankle/heel line; then square hips
- maintain orientation while upgrading handles

## 7. Failure Signatures → Fix
- **“I framed and he ran around me”** → misread as pressure when it was mobility/backward intent; switch to mobility reinsertion + re-center.
- **“He just stepped away”** → backward+pull; you failed anti-exit; follow sooner, upgrade to true handle + redundancy.
- **“I spun and got smashed”** → hands-down gate violated; base-break longer, no rotation under stable base.
- **“I keep losing the angle”** → hands are leading; re-square hips first, then reinforce with hands.
- **“Defense works but nothing changes”** → no output; force re-center or base event before progressing.

## 8. Interfaces (use-when tags)
- `open-guard_master-operating-system.md` — use when: running the full controller loop (deny link → re-center → counter).
- `decision-model_three-laws_kneeling-standing-head.md` — use when: posture context changes target selection (kneeling/standing/head height).
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: angle is forming or orientation is lost.
- `retention_framing_layer_frame-high-frame-low.md` — use when: forward+push pressure demands structure.
- `retention_movement_foot-pummeling.md` — use when: shove-to-clear / barrier removal occurs.
- `retention_movement_crossovers.md` — use when: outside knee line is forming; re-square hips.
- `retention_movement_scooting.md` — use when: you must follow retreats while staying squared.
- `application_cycle-break_to_immediate-counter.md` — use when: enforcing counter initiation immediately after cycle break.

## 9. Diagram (ASCII)

~~~
DYNAMIC ENERGY (Open Guard) = (PUSH vs PULL) x (FORWARD vs BACKWARD)

FORWARD+PUSH  -> threatens Level/Penetration/Pin  -> STRUCTURE EARLY (frames -> turn -> shrimp)
FORWARD+PULL  -> threatens Grip/Angle             -> REATTACH LEG LINE + RE-SQUARE
BACK+PUSH     -> threatens Barrier removal/reset  -> REINSERT (foot pummel) + RE-CENTER
BACK+PULL     -> threatens Reset/Disengage        -> FOLLOW + TRUE HANDLE + REDUNDANCY

GATES OVERRIDE:
HIP LINE -> DEFENSIVE CYCLE UNTIL CYCLE BREAK
NO HANDS-DOWN -> NO COMMITTED ENTRY/ROTATION
ORIENTATION -> INVARIANT (re-square before upgrading)
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Quadrant Switching (coachless)
- **Start:** passer standing; defender seated open guard.
- **Defender wins:** keep passer in front (no outside knee line) for **20s** while maintaining any contact.
- **Passer wins:** achieve **outside knee line** then **hip line touch** or **pin**.
- **Rules:** passer must alternate every ~5 seconds between “pressure forward” and “reset backward” on their own (no stalling); defender must switch modules without pausing.
- **Reset:** hip line touch / pin / timer.
- **Rounds:** 8×20s, switch.

### 10.2 No Free Reset (Backward+Pull specialization)
- **Start:** range with light contact allowed.
- **Defender wins:** establish a **true handle** and keep any contact for **15s**.
- **Passer wins:** **disengage to two steps** with no contact.
- **Rules:** passer is incentivized to backstep/flee; defender must follow with hips and upgrade to ankle/heel line.
- **Reset:** timer / disengage.
- **Rounds:** 8×20s, switch.

### 10.3 Shove-to-Clear Response (Backward+Push specialization)
- **Start:** passer standing; defender seated.
- **Defender wins:** reinsert barriers and re-center; hold “in front” for **3s**.
- **Passer wins:** achieve **outside knee line** for **3s**.
- **Rules:** passer may only shove legs aside + circle (no forward pressure); defender must reinsert first, then square.
- **Reset:** 3s hold by either side.
- **Rounds:** 8×20s, switch.

### 10.4 Pressure Ladder Entry Gate (Forward+Push + hands-down)
- **Start:** passer standing stable; defender seated open guard.
- **Defender wins:** force **post/widen/forced step** then begin a committed entry within **2s**.
- **Passer wins:** maintain stable base while advancing/clearing for **20s**.
- **Rules:** committed entry before base compromise = loss of rep; defender must base-break before “going under.”
- **Reset:** entry start after base compromise / timer.
- **Rounds:** 10 reps each, switch.

### 10.5 Strip-While-Advancing (Forward+Pull)
- **Start:** passer advances while stripping grips; defender starts with one light connection.
- **Defender wins:** reattach to leg line and re-square (opponent in front) then hold **3s**.
- **Passer wins:** achieve **outside knee line** then **hip line touch**.
- **Rules:** passer must keep stepping in (no retreats); defender prioritizes reattach first, then square (no reaching).
- **Reset:** 3s hold / hip line touch.
- **Rounds:** 8×20s, switch.