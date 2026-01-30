PATH: SYS/Guard/Open-Guard/retention_movement_inverted-spin.md

# Retention Movement — Inverted Spin (Angle Escape Under Gate)

## 1. Purpose
A retention movement system for escaping an angle loss via inversion/spin mechanics.

Key constraint: **inverted spin is only valid when the passer’s base is compromised**.  
Used correctly, it converts a near outside-knee-line loss into re-centering and barrier replacement.

Used incorrectly (under stable base), it creates immediate flattening/pin risk.

## 2. Inputs / Preconditions
- You can identify the **hands-down/base-compromise** condition.
- You can maintain some barrier/connection during the spin.
- You can finish with orientation restored (feet/knees facing) and barriers reinserted.

## 3. Outputs / Success Criteria
- Outside knee line is denied or corrected.
- You re-center with barriers rebuilt.
- Hip line threat does not increase during the spin.
- You can transition to counter start after recovery (no pause).

## 4. Core Model / Engine

### 4.1 What Inverted Spin Does
- Uses inversion to rotate the hips and legs back into an inside-facing barrier line.
- Replaces a losing angle with a squared alignment if the passer cannot immediately drive/pin.

### 4.2 Validity Condition (Hands-Down Gate)
Inverted spin requires a base-compromise signal such as:
- post/hands on mat,
- widened base that prevents immediate drive,
- forced step that breaks posture alignment.

If those are not present, treat inversion as prohibited.

### 4.3 Domain Progression Chain Hooks
Inverted spin addresses:
- **Angle** loss (outside knee line) and sometimes
- creates distance to reset barriers.

But it is a high-risk tool and must be gated.

## 5. Gates (override rules)

### 5.1 Hands-Down Gate (primary)
No inverted spin under stable base.

**Default action:** if base not compromised: use crossover/pendulum/scoot or structure based on pressure.

### 5.2 Hip Line Gate
If hip line is threatened, inversion is usually too late; use defensive cycle.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square.

### 5.3 Orientation Rule
Finish the spin with feet or knees facing opponent.

**Default action:** stop rotation as soon as facing is restored; reinsert barriers immediately.

## 6. Opponent Reactions → Responses

1) **Base recovers mid-spin (hands come off mat)**
   - Response: abort extended inversion; re-square via simpler recovery (crossover) and rebuild barriers.

2) **Passer circles to chase the spin**
   - Response: finish to facing; then re-square and reinsertion; do not keep rotating.

3) **Passer drops pressure as you invert**
   - Response: if hip line becomes threatened, switch immediately to defensive cycle (frame+turn+shrimp).

4) **Passer retreats after you recover**
   - Response: scoot-follow; upgrade to ankle/heel line true handle to deny disengage.

## 7. Failure Signatures → Fix
- **I inverted and got smashed** → hands-down gate violated; do not invert under stable base.
- **I keep rotating and lose orientation** → overspin; stop once facing returns; reinsert barriers.
- **Inversion works but I end up disconnected** → reattachment missing; follow with hips and build true handle if passer resets.
- **I invert when pressure is present** → wrong family; use structure and defensive cycle.

## 8. Interfaces (use-when tags)
- `decision-model_dynamic-energy-theory.md` — use when: hands-down gate is required for rotations/entries.
- `retention_movement_crossovers.md` — use when: angle denial is needed without inversion.
- `retention_movement_pendulum.md` — use when: late angle recovery is needed with lower risk.
- `retention_movement_scissor-roll.md` — use when: barrier replacement can be achieved via rotation without full inversion.
- `retention_framing_layer_frame-high-frame-low.md` — use when: pressure makes inversion unsafe.
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: ensuring facing is restored after recovery.

## 9. Diagram

~~~
INVERTED SPIN = HIGH-RISK ANGLE ESCAPE

trigger: near outside knee line loss + base compromised (hands-down / forced step)
action: invert/spin -> restore facing -> reinsert barriers -> re-center

hard gate:
stable base -> NO INVERSION (use crossover/pendulum/scoot or structure)

if hip line threatened -> DEFENSIVE CYCLE
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Hands-Down Gate Recognition
- **Start:** passer standing; defender seated open guard.
- **Defender wins:** only invert/spin when passer posts/hands-down; then re-center and hold **3s**.
- **Passer wins:** if defender inverts under stable base and is pinned within **5s**, or achieves **hip line touch**.
- **Rules:** passer alternates between stable base and occasional forced posts; defender must not invert unless gate appears.
- **Reset:** 3s hold / hip line touch / pin event.
- **Rounds:** 10 reps each, switch.

### 10.2 Angle Escape With Base Compromise
- **Start:** passer begins near outside knee line; defender is slightly late.
- **Defender wins:** force or use an existing base compromise, then inverted spin to re-center; hold **3s**.
- **Passer wins:** **hip line touch** or **pin**.
- **Rules:** inversion is only allowed after a visible post/widen/forced step.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 10 reps each, switch.

### 10.3 Abort Condition (base recovers mid-spin)
- **Start:** passer allows a brief post then recovers base quickly.
- **Defender wins:** begin inversion only if allowed, but abort and recover by crossover/pendulum when base returns; re-center **3s**.
- **Passer wins:** **pin** or **hip line touch**.
- **Rules:** defender must demonstrate “stop rotating when base returns.”
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 8×20s, switch.