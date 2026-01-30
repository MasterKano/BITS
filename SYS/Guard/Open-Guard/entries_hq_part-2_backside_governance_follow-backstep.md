PATH: SYS/Guard/Open-Guard/entries_hq_part-2_backside_governance_follow-backstep.md

# Entries (HQ) — Part 2: Backside Governance (Follow the Backstep, Don’t Freeze)

## 1. Purpose
Opponent’s most reliable HQ escape is the **backstep**. This module defines the governance rules to **follow the backstep** and convert it into a controllable backside entry lane rather than losing contact and restarting.

Core invariant: **your foot follows his foot** and remains a **distance governor** (center-line control) while you re-thread and turn into a stable configuration.

## 2. Inputs / Preconditions
- HQ contact exists (one of opponent’s legs is between/near your legs).
- You have at least one anchor (thread/cuff/calf contact) or can re-establish quickly.
- Opponent initiates the **backstep** (hip turns, step behind, rotation to free the line).

## 3. Outputs / Success Criteria
- You maintain contact during backstep (no disengage).
- You place your controlling foot to a **center-line target** to govern distance.
- You re-thread and turn to backside with stability.
- You deny the common follow-up escapes:
  - pull-away/disengage,
  - turn-out (toe rotation),
  - re-backstep (second backstep),
  - pressure re-collapse.

## 4. Core Model / Engine
**HQ CONTACT → BACKSTEP DETECTED → FOLLOW FOOT (center-line) → RE-THREAD → TURN TO BACKSIDE → CONSOLIDATE → ROUTE**

Operational loop:
1) Detect backstep early.
2) Place foot to center line (stomach/chest line) to prevent distance escape.
3) Follow the rotating foot; keep your knee orientation correct (no “knee to ceiling freeze”).
4) Re-thread capture from backside alignment.
5) Consolidate and route to finish/containment.

## 5. Gates (override rules)

### 5.1 Early Detection Gate (time-critical)
If you detect backstep late, you lose the line.
- **Default action:** treat hip turn + step-behind as immediate backstep cue; follow instantly.

### 5.2 Center-Line Distance Gate (primary)
Without center-line foot placement you cannot govern distance during backstep.
- **Default action:** place foot at the **center line** (stomach/chest line), then follow.

### 5.3 “No Knee-to-Ceiling Freeze” Gate (mobility)
If your knee points to the ceiling while opponent backsteps, you stop following and lose distance.
- **Default action:** keep knee oriented to allow your foot to track their foot; keep hips mobile.

### 5.4 Capture Integrity Gate (deny one-step clear)
If the opponent can clear in a single step after backstep, your re-thread is too high/thin.
- **Default action:** re-thread lower (ankle/knee line), add redundancy.

### 5.5 Collapse Threat Gate (don’t follow into pin)
If following exposes you to being flattened, you must re-insert frames first.
- **Default action:** frame high/low + turn-to-side + shrimp before re-threading.

## 6. Top-6 Situations Playbook
1) **Backstep begins as soon as you enter HQ**  
   → **Default:** follow instantly; center-line foot first.

2) **Opponent backsteps and distance increases**  
   → **Default:** you missed center-line control; re-place foot to center line and reconnect.

3) **Opponent tries a second backstep**  
   → **Default:** keep tracking; do not freeze; re-thread lower.

4) **Opponent tries turn-out/toe rotation to clear**  
   → **Default:** maintain center-line foot control and adjust to keep foot “centered” (deny toe-turn line).

5) **Opponent tries to pull away and disengage**  
   → **Default:** convert to a locking containment (bring legs together; clamp) before chasing.

6) **Opponent re-collapses into pressure**  
   → **Default:** frames first; do not follow blindly; rebuild then re-thread.

## 7. Opponent Reactions → Responses
- **Backstep:** follow foot; center-line foot placement; re-thread backside.
- **Turn-out:** keep foot centered on chest line; adjust angle; deny the toe-rotation clearance.
- **Pull-away:** lock containment (legs together / clamp) before continuing.
- **Second backstep:** continue tracking; re-thread lower; maintain redundancy.
- **Pressure collapse:** frame/angle first; then re-engage backside.

## 8. Failure Signatures → Fix
- **“He backstepped and I lost contact.”** → late detection or no center-line foot; follow earlier and place foot center-line.
- **“I froze and couldn’t track.”** → knee-to-ceiling freeze; keep knee orientation mobile.
- **“He cleared in one step after I followed.”** → thread too high; re-thread lower + redundancy.
- **“I followed and got pinned.”** → collapse threat ignored; frames first.

## 9. Trigger Recognition Checklist
Apply backside governance when 2+ cues are present:
- [ ] hip turns away from you
- [ ] stepping leg goes behind (step-behind)
- [ ] distance increases while leg rotates
- [ ] your initial thread starts to slip

## 10. Quality / Capture Checklist
- [ ] you followed early (no gap)
- [ ] foot was placed to center line during rotation
- [ ] knee did not freeze to ceiling
- [ ] re-thread denied one-step clear
- [ ] you can lock containment if pull-away begins
- [ ] you can re-insert frames if collapse begins

## 11. Interfaces (routing rules)
- `entries_hq_part-1_off-balance_to_thread-turn.md` — use when: you need the entry invariant (off-balance → thread → turn) before backstep happens.
- `entries_hq_part-3_consolidation_exit-traps_finish.md` — use when: you have tracked to backside and must consolidate/finish with exit traps.
- `governance_anti-backstep.md` — use when: backstep is the dominant escape and distance governance is the core constraint.
- `governance_anti-flee_the-mat.md` — use when: opponent’s primary defense is pull-away/disengage during the follow.
- `retention_framing_layer_frame-high-frame-low.md` — use when: follow attempts are being collapsed into pressure and frames must lead.

## 12. Diagram
~~~
HQ BACKSTEP GOVERNANCE (follow, then thread)

[HQ contact]
    |
    v
[Backstep cue: hip turn + step behind]
    |
    v
[Center-line foot placement]  (distance governor)
    |
    v
[Follow their foot]  (no knee-to-ceiling freeze)
    |
    v
[Re-thread lower + redundancy]
    |
    v
[Turn to backside stable angle]
    |
    +--> if pull-away: lock containment
    |
    +--> if collapse: frames + shrimp first
    |
    v
[Consolidate -> route to finish/containment]
~~~

## 13. Drills and Games

### 13.1 Center-Line Foot Follow
- **Start:** HQ contact; opponent immediately backsteps on cue.
- **Defender wins:** place center-line foot and maintain contact; reach backside re-thread landmark within 5s.
- **Passer wins:** complete backstep escape/disengage within 5s.
- **Rules:** any follow attempt without center-line foot placement = rep loss.
- **Reset:** landmark or escape.
- **Rounds:** 10 reps each, switch.

### 13.2 No Knee-to-Ceiling Freeze Constraint
- **Start:** opponent backsteps; coach/partner watches knee orientation.
- **Defender wins:** track foot for 5s without freezing; maintain contact.
- **Passer wins:** if defender freezes and loses contact.
- **Rules:** if knee points to ceiling during backstep, immediate rep loss.
- **Reset:** 5s hold or loss.
- **Rounds:** 8 reps each, switch.

### 13.3 Pull-Away Branch (lock before chase)
- **Start:** during follow, opponent switches from backstep to pull-away.
- **Defender wins:** convert to lock containment and prevent disengage for 3s.
- **Passer wins:** disengage to two steps within 5s.
- **Rules:** if you chase without locking when pull-away begins, rep loss.
- **Reset:** 3s hold or escape.
- **Rounds:** 8 reps each, switch.