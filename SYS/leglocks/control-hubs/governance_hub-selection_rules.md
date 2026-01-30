PATH: SYS/leglocks/control-hubs/governance_hub-selection_rules.md

# Governance — Hub Selection Rules (Inside Senkaku vs 50/50 vs Double 50 vs Criss-Cross)

## 1. Purpose
This page governs **hub selection** inside leg-entanglement exchanges. It prevents “random hub drift” by forcing explicit selection based on:
- opponent escape profile (turn-away/run, knee-line clear speed, peel/push contest),
- your current stability (knee line, contact integrity),
- and the correct escalation path (containment upgrade vs backside stability).

Output: a small set of executable routing rules.

## 2. Inputs / Preconditions
- You are in, or about to enter, a leg-entanglement hub.
- You can identify the opponent’s primary escape attempt in the last 1–2 seconds:
  - turn-away/run,
  - knee-line clear speed,
  - rotation/backstep,
  - hands-peel / legs-out push (pushing contest),
  - disengage to distance (two steps).

## 3. Outputs / Success Criteria
- You select a hub that matches the threat profile within **one decision cycle** (≤5 seconds).
- You can stabilize for **3 seconds** once selected.
- You can upgrade/downgrade hubs without losing contact integrity.

## 4. Core Model / Engine
**READ ESCAPE PROFILE → SELECT HUB → STABILIZE 3s → ROUTE (finish / upgrade / reset)**

Selection hierarchy:
1) stabilize knee line and stop the run,
2) increase containment if slipping,
3) stabilize backside pushing contests if peel/push dominates.

## 5. Gates (override rules)

### 5.1 Contact Integrity Gate (global)
If the opponent can disengage to distance in one action, selection is irrelevant until contact is restored.
- **Default action:** clamp/retain contact; if broken, re-capture (do not chase hub transitions).

### 5.2 Knee-Line Reality Gate
If knee line is not secure, “dominant hubs” are not available yet.
- **Default action:** prioritize knee-line/wedge integrity before any finishing progression.

### 5.3 Stabilize-Before-Finish Gate
Hub selection is about stability; overreaching to finish re-opens escapes.
- **Default action:** 3-second stabilization before progressing.

## 6. Top-6 Situations Playbook (selection rules)

1) **Default entry with forward-barrier available**
- **Select:** Inside Senkaku (Forward Barrier)
- **Because:** fastest stabilization when knee line can be won and turn-away can be denied.

2) **Opponent’s dominant defense is turn-away/run**
- **Select:** 50/50 (Turn-Away Containment)
- **Because:** 50/50 converts run attempts into a stable trade state.

3) **50/50 is present but clears/slips keep happening**
- **Select:** Double 50 (Multi-Leg Control)
- **Because:** you need multi-leg containment to reduce escape velocity.

4) **Exchange becomes hands-peel vs legs-out push (pushing contest)**
- **Select:** Criss-Cross (Backside Stability)
- **Because:** criss-cross solves peel-and-run by stabilizing inside/outside relationship.

5) **You cannot keep inside-senkaku seated (knee line slips)**
- **Select:** 50/50 (containment) first; upgrade to Double 50 if slipping persists.
- **Because:** containment beats chasing unstable barrier.

6) **Any hub selection repeatedly leads to disengage (two steps)**
- **Select:** Reset → re-capture (do not hub-hop).
- **Because:** contact integrity gate is failing.

## 7. Opponent Reactions → Responses (routing triggers)
- **Turn-away begins:** route to 50/50 unless inside-senkaku is already fully seated (knee line + barrier + immediate denial).
- **Knee-line clears quickly:** upgrade to double 50.
- **Rotation/backstep creates distance lane:** prefer containment hubs (50/50 → double 50) rather than barrier chasing.
- **Hands-peel dominates:** route to criss-cross stabilization.
- **Disengage to distance:** reset and re-capture; hub transitions are suspended.

## 8. Failure Signatures → Fix
- **“I keep switching hubs and losing everything.”** → stabilize-before-finish gate violated; hold 3 seconds before routing.
- **“He always runs away.”** → wrong selection; choose 50/50 earlier for turn-away profile.
- **“He clears knee line too fast.”** → upgrade delayed; go to double 50 sooner.
- **“He peels my legs and escapes.”** → pushing contest not addressed; go criss-cross sooner.
- **“He disengages to distance.”** → contact integrity gate failing; stop hub-hopping and re-capture.

## 9. Key Cues (fast classification)
- **Turn-away/run cue:** hips rotating away + immediate distance creation attempt.
- **Slip cue:** knee line retracts in one action or repeatedly.
- **Rotation cue:** backstep/hip turn repeatedly opens an exit lane.
- **Peel/push cue:** hands actively peel legs while hips push legs out to create clearance.
- **Disengage cue:** contact breaks and opponent achieves two steps of distance.

## 10. Quality / Capture Checklist
- [ ] I named the escape profile before choosing a hub
- [ ] I chose the hub that solves that profile (not my preference)
- [ ] I stabilized 3 seconds before progressing
- [ ] I upgraded (double 50) only when slipping persisted
- [ ] I used criss-cross when peel/push dominated
- [ ] I reset when contact integrity failed

## 11. Interfaces (routing rules)
- `SYS/leglocks/control-hubs/hub_inside-senkaku_forward-barrier.md` — use when: forward barrier + knee line can be secured quickly.
- `SYS/leglocks/control-hubs/hub_50-50_turn-away-containment.md` — use when: turn-away/run is dominant or barrier is unstable.
- `SYS/leglocks/control-hubs/hub_double-50_multi-leg-control.md` — use when: 50/50 slips and knee-line clears persist.
- `SYS/leglocks/control-hubs/hub_criss-cross_inside-outside_backside-stability.md` — use when: pushing contest (hands peel vs legs push) dominates.
- `SYS/leglocks/defence/knee-line-and-wedge-control.md` — use when: knee-line integrity is the key failure point.

## 12. Diagram
~~~
HUB SELECTION (Rule Ladder)

Read profile (last 1–2s):
  A) turn-away/run?
  B) knee-line clears fast?
  C) peel/push contest?
  D) disengage to distance?

Routing:
  if disengage -> RESET / re-capture (no hub)
  else if peel/push -> CRISS-CROSS
  else if clears persist -> DOUBLE 50
  else if turn-away -> 50/50
  else -> INSIDE SENKAKU (default)
~~~

## 13. Drills and Games

### 13.1 Name-the-Profile → Pick-the-Hub
- **Start:** partner chooses one profile (run / slip / peel-push / disengage) and acts immediately.
- **Defender wins:** name the profile and select the correct hub within 5s, then hold 3s.
- **Passer wins:** escape (disengage to two steps) within 5s.
- **Rules:** wrong hub selection = rep loss.
- **Reset:** 3s hold or escape.
- **Rounds:** 12 reps each, switch.

### 13.2 Upgrade Timing (50/50 → double 50)
- **Start:** 50/50 is present; opponent attempts repeated knee-line clears.
- **Defender wins:** upgrade to double 50 on the first clear attempt and stabilize 3s.
- **Passer wins:** clear and disengage within 5s.
- **Rules:** do not overreach; stabilize first.
- **Reset:** 3s hold or escape.
- **Rounds:** 10 reps each, switch.