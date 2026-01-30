PATH: SYS/leglocks/control-hubs/hub_double-50_multi-leg-control.md

# Hub — Double 50: Multi-Leg Control (Upgrade Containment When 50/50 Slips)

## 1. Purpose
Double 50 is a leg-entanglement **containment upgrade**: it exists to solve the primary failure mode of 50/50 and similar hubs—**repeated knee-line clears and slippery rotation exits**.

Operational intent:
- increase containment by controlling **multiple leg lines**,
- reduce escape velocity (turn-away/backstep/pull-away),
- stabilize to a point where finishing routes become systematic.

## 2. Inputs / Preconditions
- You are already in a leglock exchange where one-leg containment is insufficient:
  - 50/50 is seated but opponent keeps clearing/rotating,
  - inside-senkaku is unstable (knee line slips),
  - scrambles repeatedly return to “almost contained.”
- You can access additional leg control without losing hip-line safety.

## 3. Outputs / Success Criteria
You are “in hub” when:
- the opponent cannot clear to distance in one action,
- knee line retraction is materially slowed (requires multi-step effort),
- you can hold containment **3 seconds** while maintaining routing options,
- you can route cleanly to:
  - finishing systems, or
  - criss-cross stability if backside contests dominate.

## 4. Core Model / Engine
**ARRIVE (slip detected) → UPGRADE TO MULTI-LEG CONTROL → DENY CLEAR/ROTATION → CONSOLIDATE → ROUTE / FINISH**

Key idea: when one-leg containment is unreliable, you win by **owning the second leg line** so rotation and step-clears are no longer free.

## 5. Gates (override rules)

### 5.1 Upgrade Gate (when to choose double 50)
If the opponent clears knee line quickly or repeatedly, you must upgrade.
- **Default action:** transition from single-line containment to multi-leg containment immediately.

### 5.2 Integrity Gate (do not sacrifice primary containment to chase the second leg)
If upgrading causes you to lose the original entanglement, you downgraded.
- **Default action:** keep the first leg controlled; add the second without opening the escape lane.

### 5.3 Turn-Away / Rotation Gate
If the opponent’s rotation creates distance, containment failed.
- **Default action:** follow rotation while keeping multi-leg connection; re-seat before attacking.

### 5.4 Pull-Away Gate
If contact breaks and opponent disengages to two steps, you failed containment.
- **Default action:** clamp/contain first; if lost, route to re-capture rather than chase.

### 5.5 “Stabilize Before Finish” Gate
Double 50 is an upgrade hub; overreaching re-opens escapes.
- **Default action:** stabilize 3 seconds, then progress.

## 6. Top-6 Situations Playbook
1) **50/50 is seated but opponent clears knee line repeatedly**  
   → **Default:** upgrade to double 50.

2) **Opponent is slippery and rotates out of inside-senkaku**  
   → **Default:** upgrade containment via second leg line control.

3) **Opponent’s main defense is turn-away/run**  
   → **Default:** upgrade so rotation cannot create distance.

4) **Opponent’s defense becomes a backside pushing contest**  
   → **Default:** route to criss-cross stability once multi-leg control is achieved.

5) **Opponent pull-aways as you progress**  
   → **Default:** containment first; if contact breaks, route to distance re-capture.

6) **You have stable multi-leg containment**  
   → **Default:** proceed to finishing routes or improve position per hub-selection rules.

## 7. Opponent Reactions → Responses
- **Knee-line clear attempts:** add/maintain multi-leg control; deny one-step clear; re-seat lower.
- **Turn-away/rotation:** follow rotation with both legs controlled; prevent distance creation.
- **Backstep/hip turn:** track hips; maintain multi-leg connection; re-seat before advancing.
- **Pull-away:** clamp; if disengage occurs, route to re-capture systems.
- **Hand-fight/strip:** preserve structural control; replace grips only if containment remains.

## 8. Failure Signatures → Fix
- **“I tried to upgrade and lost everything.”** → integrity gate violated; maintain primary leg first.
- **“He still clears fast.”** → you upgraded too late or too shallow; commit to multi-leg control earlier.
- **“I overreached and he ran.”** → stabilize-before-finish gate violated; hold 3 seconds, then progress.
- **“He disengaged to distance.”** → pull-away gate violated; clamp earlier or route immediately on break.

## 9. Key Cues

### 9.1 Permission Cues (upgrade now)
- knee line clears are frequent and fast,
- opponent’s rotation repeatedly creates escape lanes,
- 50/50 feels like “temporary contact,” not containment.

### 9.2 Abort Cues (route away)
- upgrading causes loss of primary leg control,
- you cannot prevent disengage to two steps,
- you are being flattened and cannot re-angle.

### 9.3 Success Landmarks
- opponent cannot clear in one action,
- rotation stalls (does not create distance),
- 3-second stable hold available with routing options intact.

## 10. Quality / Capture Checklist
- [ ] upgraded because of repeated slip/clear (not by habit)
- [ ] primary leg line never sacrificed during upgrade
- [ ] rotation does not create distance
- [ ] one-step clear is denied
- [ ] 3-second stable hold available
- [ ] clear route to finish or criss-cross stability

## 11. Interfaces (routing rules)
- `SYS/leglocks/control-hubs/hub_50-50_turn-away-containment.md` — use when: single-line containment is working; upgrade only when clears/slips persist.
- `SYS/leglocks/control-hubs/hub_criss-cross_inside-outside_backside-stability.md` — use when: backside pushing contests dominate and you need stabilized inside/outside control.
- `SYS/leglocks/control-hubs/governance_hub-selection_rules.md` — use when: deciding between 50/50, double 50, criss-cross based on escape profile.
- `SYS/leglocks/defence/knee-line-and-wedge-control.md` — use when: knee-line integrity is the failure point and wedge control is required.
- `SYS/leglocks/transitions/backside-50-50.md` — use when: rotational escapes force backside containment transitions.

## 12. Diagram
~~~
DOUBLE 50 HUB (Multi-Leg Control)

[Slip detected in 50/50 or senkaku]
          |
          v
[Upgrade]
(keep primary leg + add second leg line)
          |
          v
[Deny exits]
knee-line clear -> deny one-step
rotation/run    -> follow; prevent distance
pull-away       -> clamp or route
          |
          v
[Stabilize 3s]
          |
          v
[Route]
-> finish system
-> criss-cross (if backside contest)
~~~

## 13. Drills and Games

### 13.1 Upgrade-on-Slip Timer
- **Start:** seated 50/50; opponent’s only goal is fast knee-line clear.
- **Defender wins:** upgrade to double 50 within 5s and hold 3s.
- **Passer wins:** clear/disengage within 5s.
- **Rules:** upgrade must keep original leg control (no “let-go then chase”).
- **Reset:** 3s hold or escape.
- **Rounds:** 10 reps each, switch.

### 13.2 Rotation Containment Reps
- **Start:** double 50 seated; opponent’s only goal is turn-away/rotation to create distance.
- **Defender wins:** prevent distance escape for 5s and hold 3s at any point.
- **Passer wins:** disengage to two steps within 5s.
- **Rules:** stabilize before any finishing attempt.
- **Reset:** timer/hold or escape.
- **Rounds:** 8 reps each, switch.

### 13.3 Decision Route (double 50 vs criss-cross)
- **Start:** double 50 seated; opponent alternates between knee-line clear attempts and backside pushing contests.
- **Defender wins:** choose correct route within 5s (stay double 50 or shift to criss-cross), then hold 3s.
- **Passer wins:** escape within 5s.
- **Rules:** wrong route choice = rep loss.
- **Reset:** 3s hold or escape.
- **Rounds:** 10 reps each, switch.