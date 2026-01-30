# Constraint gates

## Purpose

Define the **permission gates** that must be satisfied before committing to large transitions (stand-ups, rolls, backtakes, forward pressure). If a constraint is active, solve it first.

## Core idea

- Transitions fail because you moved while **permission was not granted**.
- A gate is “passed” when:
  - your leg line is safe,
  - the opponent’s controlling constraint is neutralized,
  - and your next action will not immediately create exposure or lose connection.

## ASCII gate flow

~~~text
{ABOUT TO TRANSITION}
        |
        v
{ACTIVE CONSTRAINT?} -- no --> EXECUTE TRANSITION
        |
       yes
        |
        v
IDENTIFY CONSTRAINT -> APPLY FIX -> RECHECK GATE -> EXECUTE
~~~

## Constraint list (canonical)

### A) Achilles / foot control constraint
- Opponent has an effective Achilles/foot grip that prevents forward pressure, knee-down, or safe stand/roll.

### B) Heel-line exposure constraint
- Your heel becomes available during movement (stand, roll, pummel, inversion exchange).

### C) Wedge / knee-line constraint (inside ashi / 50-50)
- Structural wedge prevents coming forward; knee-line is trapped; separation is blocked.

### D) Head-line constraint (back connectors)
- Head-and-arm / head-line is slipping; opponent is walking head out and re-squaring.

### E) Inversion constraint
- Opponent initiates inversion to create leg-line threats or to escape; ankle/leg line must be managed early.

### F) “Belly-down sitback” constraint (top ushiro failure state)
- Opponent gets your chest flat and sits back on hips while belly-down, trapping your knee/leg line.

## Permission gates (checklists)

### 1) Foot safety gate
- Foot is hidden (orientation denies current primary threat).
- Heel-line is not presented during the movement you are about to do.
- You can move without your foot drifting closer into their control space.

### 2) Achilles constraint gate
- Opponent’s Achilles grip is neutralized OR no longer functionally limiting your next action.
- You are not committing to high-amplitude movement (stand/roll/drive) while Achilles control is active.

### 3) Wedge / knee-line gate (inside ashi / 50-50)
- You created space with a post/pummel OR transferred to a configuration that re-enables offense (outside/cross).
- You are not forcing forward pressure into a structural block.

### 4) Head-line gate (back connector)
- Head-and-arm clamp is tight enough that they cannot walk head out.
- You are not chasing hooks while the head line is slipping.

### 5) Inversion gate
- You have an early anchor (post/pin on ankle/leg line) before chasing position.
- Your own leg line is protected during pummeling/rotation (do not trade safety for movement).

### 6) Top ushiro emergency gate
- Foot is hidden first.
- Knee/leg line extraction is initiated immediately.
- You have a drive leg/base to complete extraction (do not attempt extraction without a drive leg).

## Decision rules (IF/THEN)

- IF Achilles/foot control is active -> THEN treat forward pressure as constrained; clear/deny it or change lane.
- IF heel-line exposure is developing -> THEN foot hide + leg extraction before any conversion goal.
- IF wedge blocks forward motion -> THEN do not force forward; post/pummel or transfer to outside/cross; use roll families.
- IF inversion begins -> THEN post/pin ankle early; manage inversion at initiation, not late.
- IF head line is slipping during a back connector -> THEN tighten clamp and re-close head line before hook pursuit.
- IF chest is flattened and opponent sits back on hips (top ushiro disaster state) -> THEN emergency: hide foot, extract knee line, regain drive leg.

## Failure signatures + fixes

- Failure: stand/roll/drive → immediate heel exposure.
  - Fix: re-run Foot safety gate; do not transition until heel-line risk is controlled.
- Failure: you chase a backtake while Achilles control is active → stall/exposure.
  - Fix: solve Achilles constraint first or switch to pin/passing lane.
- Failure: you force forward into a wedge → no progress.
  - Fix: post/pummel or transfer; do not “drive harder.”
- Failure: you wait until inversion is fully formed.
  - Fix: anchor early (ankle post/pin), then re-enter.
- Failure: head walks out during backtake connector.
  - Fix: shrink the circle and re-close head line before advancing.
- Failure: top ushiro collapses into chest-flat sitback.
  - Fix: emergency sequence immediately—foot hide → knee extraction → rebuild base.

## Completion checks

- You can name:
  - the active constraint,
  - the gate you’re satisfying,
  - and the first control you will establish after the transition.
- Your transition does not produce immediate:
  - heel exposure,
  - loss of head-line connection,
  - or loss of positional advantage.

## Links

- `conversion-loop.md`
- `cranial-shift.md`
- `back-completion-criteria.md`

## Sources

- Gordon Ryan — Pillars of Defense: Leg Locks to Back Takes
  - `INS/gr-pod/VN/v1.md`
  - `INS/gr-pod/VN/v4.md`
  - `INS/gr-pod/VN/v5.md`
  - `INS/gr-pod/VN/v6.md`
