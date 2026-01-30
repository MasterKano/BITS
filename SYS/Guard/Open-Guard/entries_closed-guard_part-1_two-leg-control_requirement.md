PATH: SYS/Guard/Open-Guard/entries_closed-guard_part-1_two-leg-control_requirement.md

# Entries (Closed Guard) — Part 1: Two-Leg Control Requirement (No “Hope Close”)

## 1. Purpose
In no-gi open guard, “closing guard” is often attempted as a convenience—but against competent posture and movement it fails unless you satisfy one binding requirement:

**You must control both legs (or both sides of the opponent’s base) before you close.**

This module defines what counts as two-leg control, why one-leg-only closes fail, and how to route when the requirement is not met (stay open guard, switch entries, or move into X/ashi/hub routes).

## 2. Inputs / Preconditions
- Opponent is standing or transitioning through standing.
- You are in open guard and can attempt to connect your legs around the opponent’s hips/waistline.
- You can maintain hip-line safety (not being flattened during the attempt).

## 3. Outputs / Success Criteria
- You achieve a **true closed-guard close** where:
  - opponent cannot immediately stand tall and open,
  - opponent cannot immediately backstep/step-clear and disengage,
  - you have an attack-ready structure (angles, posture control, or entry route).
- You only attempt closure when the **two-leg requirement** is satisfied.

## 4. Core Model / Engine
**TWO-LEG CONTROL → HIP LINE SAFE → CLOSE → IMMEDIATE GOVERNANCE (posture/angle) → ROUTE**

Operational logic:
- Closed guard is not a “position you arrive at”; it is a **state you are allowed to lock** when the opponent’s base is already constrained.

## 5. Gates (override rules)

### 5.1 Two-Leg Control Gate (primary)
If you do not control both legs, you are not allowed to close.
- **Default action:** remain in open guard; build the second-leg control (or switch to a different entry family).

### 5.2 Anti-Backstep Gate (common failure mode)
If the opponent can backstep while you’re trying to close, you will lose position.
- **Default action:** maintain distance governance (foot tracking / center-line control) and do not close until backstep is denied.

### 5.3 Anti-Stand-Tall Gate (posture opening)
If the opponent can stand tall freely, your close will be opened immediately.
- **Default action:** do not close; create posture compromise first (base event) or keep open guard entries.

### 5.4 Hip Line Safety Gate (no closing while being collapsed)
If closing exposes you to being flattened, you must defend first.
- **Default action:** frames high/low + turn-to-side + shrimp → rebuild → resume.

## 6. Top-6 Situations Playbook
1) **You have one leg (single-line control) but want to close**  
   → **Default:** do not close; acquire second leg or route to X/ashi entry.

2) **Opponent is standing tall and balanced**  
   → **Default:** closure is illegal; create base event or attack legs at distance.

3) **Opponent is staggered and you can control near + far leg**  
   → **Default:** requirement satisfied; close and immediately govern posture/angle.

4) **Opponent begins to backstep as you connect**  
   → **Default:** abort closure; track foot; deny backstep; then reattempt only if two-leg control remains.

5) **Opponent pulls away / disengages**  
   → **Default:** do not chase closure; route to shin-to-shin / 2-on-1 ankle re-capture.

6) **You obtain two-leg control but are being collapsed**  
   → **Default:** safety first; frames and angle, then close only from stable hip line.

## 7. Opponent Reactions → Responses
- **Backstep:** track stepping foot; keep distance governor; do not close.
- **Stand tall:** treat as failed condition; switch to distance entries or off-balance first.
- **Pull away:** route immediately to distance connectors; do not “run after a close.”
- **Pressure collapse:** frames/angle first; re-enter when safe.
- **Knee-line clearing (one leg steps free):** you’ve lost the requirement; remain open guard.

## 8. Failure Signatures → Fix
- **“I closed and he instantly opened and passed.”** → you closed without two-leg control; enforce Gate 5.1.
- **“He backstepped as I tried to close.”** → anti-backstep not satisfied; track/deny first.
- **“He stood up and my close failed.”** → anti-stand-tall not satisfied; create base event or stay open.
- **“I got flattened trying to close.”** → hip line safety violated; defend first.

## 9. Trigger Recognition Checklist
You may close when 2+ are true:
- [ ] both legs are controlled (or base is constrained on both sides)
- [ ] opponent cannot freely backstep/step-clear
- [ ] opponent’s posture is not fully tall/stable
- [ ] your hip line is safe (not being collapsed)

## 10. Quality / Capture Checklist
- [ ] your closure is built off two-leg control, not timing luck
- [ ] you have immediate posture/angle governance upon closing
- [ ] opponent’s first escape (backstep/stand tall/pull-away) is already denied
- [ ] you can route immediately to Part 2 (closed-to-X bridge) if they begin to open

## 11. Interfaces (routing rules)
- `entries_closed-guard_part-2_closed-to-x-guard_bridge.md` — use when: you close under governance and need the standard conversion as they begin to open.
- `entries_distance_2-on-1-ankle-system.md` — use when: opponent stands tall or disengages; you must re-capture at distance.
- `entries_distance_shin-to-shin_connector.md` — use when: you need mid-range re-attachment after pull-away.
- `entries_x-guard_triple-attack.md` — use when: two-leg control is easier to achieve via X-guard pathways than direct closing.
- `governance_anti-backstep.md` — use when: backstep is the primary denial against closing attempts.
- `governance_anti-flee_the-mat.md` — use when: opponent’s primary defense is disengage/pull-away during closure attempts.

## 12. Diagram
~~~
CLOSED GUARD ENTRY (No-Gi) = PERMISSIONED BY TWO-LEG CONTROL

[Open guard contact]
       |
       v
[Two-leg control?] --no--> [Stay open: build 2nd leg / route to distance or X/ashi]
       |
      yes
       v
[Hip line safe?] --no--> [Frames/turn/shrimp -> rebuild]
       |
      yes
       v
[CLOSE]
       |
       v
[Immediate governance]
(deny backstep / deny stand-tall / create angle)
       |
       v
[Route]
-> Part 2 closed-to-X bridge
-> or resume open guard entries if close breaks
~~~

## 13. Drills and Games

### 13.1 Two-Leg Permission Game
- **Start:** open guard; opponent standing. Defender may attempt to close at any time.
- **Defender wins:** close only after two-leg control and hold closed guard 3s.
- **Passer wins:** if defender closes without two-leg control and passer opens + disengages within 5s.
- **Rules:** any “illegal close” (no two-leg control) is automatic rep loss.
- **Reset:** 3s hold or 5s escape.
- **Rounds:** 10 reps each, switch.

### 13.2 Backstep Denial Before Close
- **Start:** defender has near-leg control; opponent’s job is to backstep whenever defender connects legs.
- **Defender wins:** deny backstep by tracking/controlling both legs, then close legally for 3s.
- **Passer wins:** successful backstep escape within 5s.
- **Rules:** defender must demonstrate both-leg constraint before closing.
- **Reset:** 3s hold or escape.
- **Rounds:** 8 reps each, switch.

### 13.3 Stand-Tall Punisher (don’t close on stable posture)
- **Start:** opponent begins tall and balanced; defender has partial attachments.
- **Defender wins:** create a base event (post/step/widen) and acquire two-leg control; then close 3s.
- **Passer wins:** remain tall/balanced for 10s or open and disengage within 5s after a close attempt.
- **Rules:** closing into tall, stable posture is rep loss.
- **Reset:** 3s hold or timer/escape.
- **Rounds:** 8 reps each, switch.