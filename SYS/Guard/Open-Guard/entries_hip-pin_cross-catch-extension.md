PATH: SYS/Guard/Open-Guard/entries_hip-pin_cross-catch-extension.md

# Entries — Hip Pin off Cross-Catch / Irimi Ashi Defence (Knee-on-Hip Pin → Backstep Access)

## 1. Purpose
When your opponent becomes “smart” and defends the backstep-lace entry by **sitting to a hip and a hand**, you switch from elevation-based catching to **hip-pin control**: pull up, place **knee on hip**, perch weight over them so standing is difficult, then use a backstep line to enter the legs (sit-back or roll-forward options described).

## 2. Inputs / Preconditions
- You have entered via Irimi/Ashi connection and opponent is defending by **dropping hip to floor** (hip + hand posting).
- You can follow them up (come upright) rather than insisting on elevation.
- You can place your **knee on their hip** with meaningful weight.

## 3. Outputs / Success Criteria
- Opponent’s hip is **pinned** (standing/escaping becomes difficult).
- You can create a clean backstep line over/around their leg depending on knee direction.
- You can enter into legs from the pin via:
  - sitting back, or
  - rolling forward,
  while maintaining control.

## 4. Core Model / Engine
**DEFENCE DETECTED (hip sit) → FOLLOW UP → KNEE-ON-HIP PIN → CHOOSE BACKSTEP LINE → ENTER LEGS (sit-back / roll-forward)**

Two steering reads:
- If opponent’s **knee points toward you**: backstep over it.
- If opponent’s **knee points away**: use foot-to-hand pull to bring it into a controllable line, then lock.

## 5. Gates (override rules)

### 5.1 “Hip Sit” Recognition Gate
This system is a response to the hip-sit defence; don’t force it if opponent is still balanced high.
- **Default action:** continue the prior elevation/backstep-lace system until the hip sit appears.

### 5.2 Weight-on-Hip Gate (pin quality)
If your pin has no weight, opponent stands too easily.
- **Default action:** perch your weight over hip before attempting the backstep entry.

### 5.3 Knee-Direction Gate (entry selection)
Your backstep path depends on the opponent’s knee direction.
- **Default action:** read knee direction first; then pick the correct backstep line.

## 6. Top-6 Situations Playbook
1) **Opponent sits to hip + hand as you attempt elevation**  
   → **Default:** follow up; do not insist on elevation.

2) **You are upright over them**  
   → **Default:** knee-on-hip pin; perch weight.

3) **Opponent tries to stand**  
   → **Default:** increase weight over hip; standing becomes difficult.

4) **Opponent knee points toward you**  
   → **Default:** backstep directly over the knee.

5) **Opponent knee points away**  
   → **Default:** foot-to-hand pull to bring knee into a controllable line, then lock.

6) **Entry moment appears**  
   → **Default:** choose sit-back or roll-forward entry into legs.

## 7. Opponent Reactions → Responses
- **Hip sits:** switch to pin.
- **Tries to stand:** increase weight over pinned hip; keep posture perched.
- **Knee rotates away:** use foot-to-hand pull option to fix the line.
- **Knee points in:** backstep directly.
- **Frames/hand posts:** keep perch; enter legs on timing when their hip is trapped.

## 8. Failure Signatures → Fix
- **“He stood right up.”** → your pin lacked weight; perch more over the hip.
- **“I backstepped the wrong way and lost the line.”** → you skipped knee-direction read; select path based on knee pointing toward/away.
- **“I tried to elevate even though he sat.”** → wrong tool; this defence is designed to beat the elevation entry.

## 9. Trigger Recognition Checklist
Switch to hip-pin when:
- [ ] opponent sits hip to floor with a hand post
- [ ] elevation feels “shut down” by their low hips
- [ ] you can come upright enough to pin hip with knee

## 10. Quality / Capture Checklist
- [ ] knee is on hip with real weight
- [ ] opponent cannot stand easily
- [ ] knee-direction read is clear (toward vs away)
- [ ] you have a defined entry choice (sit-back or roll-forward)

## 11. Interfaces (routing rules)
- `entries_cross-catch_irimi-ashi.md` — use when: you are still in the elevation/backstep-lace phase and opponent has not hip-sat yet.
- `entries_kneeling_reverse-double-entry.md` — use when: you regain close contact around waist and can collect two legs instead.
- `governance_anti-flee_the-mat.md` — use when: opponent’s primary escape is to run/turn away as you enter.
- `governance_hub-selection_rules.md` — use when: you land in a leg-control position and must choose stabilization hub.

## 12. Diagram
~~~
HIP-PIN RESPONSE TO HIP-SIT DEFENCE

[Irimi/Ashi entry attempt]
        |
        v
[Opponent sits to hip + hand]  (defence)
        |
        v
[Follow up / come upright]
        |
        v
[Knee ON hip + perch weight]
        |
        +--> knee points TOWARD you -> backstep over knee
        |
        +--> knee points AWAY -> foot-to-hand pull -> lock
        |
        v
[Enter legs]
(sit-back OR roll-forward)
~~~

## 13. Drills and Games

### 13.1 Hip-Sit Recognition + Pin
- **Start:** begin from Irimi/Ashi connect; partner defends by hip-sitting on cue.
- **Defender wins:** follow up and establish knee-on-hip pin with weight; hold 3s.
- **Passer wins:** stand up fully or disengage before 3s.
- **Rules:** no elevation attempts after hip sit; must switch to pin immediately.
- **Reset:** 3s hold or escape.
- **Rounds:** 10 reps each, switch.

### 13.2 Knee-Direction Decision Game
- **Start:** knee-on-hip pin achieved; partner alternates knee pointing toward/away.
- **Defender wins:** choose correct path (backstep over vs pull-and-lock) and reach leg-entry position within 5s.
- **Passer wins:** clear the pin or stand within 5s.
- **Rules:** you must verbalize (internally) the read before moving; no guessing.
- **Reset:** entry or escape.
- **Rounds:** 8 reps each, switch.

### 13.3 Sit-Back vs Roll-Forward Choice
- **Start:** knee-on-hip pin; you are “cleared” to enter.
- **Defender wins:** hit either sit-back or roll-forward entry cleanly and maintain control 3s.
- **Passer wins:** break pin and disengage.
- **Rules:** alternate choice each rep (rep 1 sit-back, rep 2 roll-forward, etc.).
- **Reset:** 3s hold or escape.
- **Rounds:** 8 reps each, switch.