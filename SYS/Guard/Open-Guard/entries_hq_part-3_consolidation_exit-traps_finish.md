PATH: SYS/Guard/Open-Guard/entries_hq_part-3_consolidation_exit-traps_finish.md

# Entries (HQ) — Part 3: Consolidation + Exit Traps + Finish (Don’t “Arrive and Drift”)

## 1. Purpose
Once you’ve entered and/or followed HQ into a workable line (often backside after backstep), the deciding phase is **consolidation**: converting a momentary capture into a stable control state that prevents the opponent’s last-ditch exits.

This module defines:
- what “consolidated” means in HQ-derived entries,
- the primary exit attempts (backstep again, pull-away, toe-turn/turn-out, knee-close, pressure re-collapse),
- the executable **exit traps** that keep you attached long enough to complete your downstream system.

## 2. Inputs / Preconditions
- You have reached one of these states:
  - HQ thread with a real capture (denies one-step clear), or
  - backside follow state after the opponent backsteps (HQ Part 2), or
  - partial leg-entry state where heel/ankle line is in reach but not yet locked.
- You can maintain at least one hard anchor:
  - leg line capture (ankle/knee line), or
  - center-line distance foot, or
  - clamp/containment with legs together.
- You can feel whether the opponent is trying to:
  - **withdraw** (pull-away/disengage), or
  - **rotate** (turn-out/toe rotation/backstep again), or
  - **collapse** (pressure back into you).

## 3. Outputs / Success Criteria
You are “consolidated” when:
- you deny the opponent’s next exit attempt for **≥3 seconds**, and
- your capture cannot be cleared in one step, and
- you have an immediate route to a downstream hub/finish system without re-gripping from scratch.

Operational outcomes:
- exit trap triggers correctly on first cue,
- you maintain distance governance during rotation,
- you can transition to: criss-cross / double 50 / 50-50 / inside-senkaku, or to the appropriate continuation module.

## 4. Core Model / Engine
**ARRIVE (capture) → IDENTIFY EXIT TYPE → APPLY EXIT TRAP → RE-LOCK → ROUTE / FINISH**

Exit types:
- **Backstep escape** (hip turns; step behind)
- **Pull-away disengage** (hip withdrawal; distance increase)
- **Turn-out / toe rotation** (toe turns away; knee line clears)
- **Knee-close / leg closure** (knees pinch; pummel lane dies)
- **Pressure re-collapse** (chest-to-chest/pin attempt)

Exit traps are not “moves”; they are **default reactions** that preserve your anchors.

## 5. Gates (override rules)

### 5.1 Consolidation Gate (no finishing before lock)
If you have not achieved a lock state, “finish chasing” will get you detached.
- **Default action:** prioritize exit traps and re-lock before advancing.

### 5.2 One-Step Clear Gate (capture integrity)
If the opponent can clear the capture in a single step, you are not consolidated.
- **Default action:** thread lower + add redundancy; bring legs together to clamp if needed.

### 5.3 Center-Line Distance Gate (rotation/backstep control)
Rotation-based exits must be governed by center-line foot placement.
- **Default action:** foot to center line; follow foot; keep it centered on chest/stomach line.

### 5.4 Pull-Away Gate (lock before chase)
Chasing a withdrawing opponent without locking is a loss condition.
- **Default action:** clamp/contain (legs together, knee-to-floor if applicable) before any pursuit.

### 5.5 Collapse Threat Gate (frames first)
If opponent turns consolidation into pressure, entry work pauses.
- **Default action:** frame high/low + turn-to-side + shrimp → rebuild → re-engage.

## 6. Top-6 Situations Playbook
1) **You’ve arrived to backside and opponent begins a second backstep**  
   → **Default:** center-line foot immediately; follow foot; re-thread lower; deny one-step clear.

2) **Opponent tries to pull away and disengage**  
   → **Default:** clamp/contain first (legs together / lock), then route.

3) **Opponent tries toe-turn / turn-out**  
   → **Default:** keep foot centered; deny toe rotation line; keep knee line protected.

4) **Opponent pinches knees to kill threading**  
   → **Default:** post/structure to keep knees apart; then re-thread lower.

5) **Opponent collapses pressure into you mid-consolidation**  
   → **Default:** frames first; re-square; re-enter when hip line is safe.

6) **You have a stable lock**  
   → **Default:** route immediately to the correct hub/finish system; do not linger in HQ.

## 7. Opponent Reactions → Responses (Exit Traps)
- **Backstep again:** center-line foot + follow-foot; re-thread lower; keep knee mobile (no freeze).
- **Pull-away:** clamp/contain; deny two-step disengage; then route.
- **Turn-out/toe rotation:** keep foot centered on chest line; adjust angle to deny toe line; reinforce knee-line safety.
- **Knee-close:** second-hand post to keep knees apart; re-thread lower.
- **Pressure collapse:** frames/turn/shrimp; re-enter after hip line is safe.

## 8. Failure Signatures → Fix
- **“I got there but he just stepped out.”** → one-step clear existed; thread lower + redundancy before advancing.
- **“He backstepped again and I lost him.”** → no center-line distance governance; place foot center-line earlier.
- **“He ran away as I tried to finish.”** → you chased without locking; clamp/contain first.
- **“I got flattened trying to consolidate.”** → collapse threat ignored; frames first, then re-engage.
- **“My threading dies when knees pinch.”** → you skipped the knees-apart post; prevent knee-close first.

## 9. Trigger Recognition Checklist
Apply exit traps when 2+ cues appear:
- [ ] hip turn begins (backstep cue)
- [ ] distance increases (pull-away cue)
- [ ] toe points away / knee line rotates (turn-out cue)
- [ ] knees pinch together (knee-close cue)
- [ ] chest pressure starts to consolidate (collapse cue)

## 10. Quality / Capture Checklist
You are consolidated when:
- [ ] one-step clear is denied
- [ ] at least one hard anchor remains during exit attempts
- [ ] center-line distance governance is available during rotation/backstep
- [ ] pull-away is stopped before chase (clamp/contain)
- [ ] you can route immediately to a hub/finish without re-gripping from scratch

## 11. Interfaces (routing rules)
- `entries_hq_part-1_off-balance_to_thread-turn.md` — use when: you need HQ entry invariants before consolidation matters.
- `entries_hq_part-2_backside_governance_follow-backstep.md` — use when: the main battle is tracking the backstep to reach a consolidatable state.
- `governance_anti-backstep.md` — use when: backstep is the primary exit you must trap during consolidation.
- `governance_anti-flee_the-mat.md` — use when: pull-away/disengage is the primary exit.
- `hub_criss-cross_inside-outside_backside-stability.md` — use when: you end backside and need pushing-dominant stabilization.
- `hub_double-50_multi-leg-control.md` — use when: you need multi-leg containment to stop repeated exits.
- `hub_50-50_turn-away-containment.md` — use when: classic containment is the correct fallback after consolidation.
- `hub_inside-senkaku_forward-barrier.md` — use when: you can establish a forward barrier and want maximum control before finishing.

## 12. Diagram
~~~
HQ PART 3: CONSOLIDATION + EXIT TRAPS

[Arrive w/ capture]  (HQ thread or backside follow)
          |
          v
[Exit-type ID]
 backstep | pull-away | turn-out | knee-close | collapse
    |         |          |           |           |
    v         v          v           v           v
[Trap]     [Clamp]   [Center]     [Knees]     [Frames]
center     lock       foot         apart       first
line       first      centered     + rethread  (turn/shrimp)
follow     then       deny toe     lower
    \         |          |           |           /
     \        v          v           v          /
      +---->[RE-LOCK / CONSOLIDATE]------------+
                     |
                     v
               [ROUTE / FINISH]
   (criss-cross / double 50 / 50-50 / inside senkaku)
~~~

## 13. Drills and Games

### 13.1 Exit-Type Randomization (trap selection)
- **Start:** you begin from a “nearly consolidated” HQ/backside capture.
- **Defender wins:** correctly stop the chosen exit (backstep OR pull-away OR turn-out OR knee-close) for 3s, then route to a hub landmark.
- **Passer wins:** complete the chosen exit within 5s.
- **Rules:** opponent chooses one exit per rep and commits; defender must respond with the correct default trap first (no finishing attempts until 3s control).
- **Reset:** 3s hold + route landmark, or 5s escape.
- **Rounds:** 12 reps each, switch.

### 13.2 One-Step Clear Audit (capture integrity)
- **Start:** defender claims they are consolidated; opponent tries only one-step clear.
- **Defender wins:** deny one-step clear for 5s (thread lower + redundancy if needed).
- **Passer wins:** one-step clear within 5s.
- **Rules:** defender must fix by re-threading lower (no chasing hands).
- **Reset:** 5s hold or clear.
- **Rounds:** 8 reps each, switch.

### 13.3 Pull-Away Trap (lock before chase)
- **Start:** from backside/HQ capture; opponent immediately pull-aways.
- **Defender wins:** clamp/contain first, prevent disengage for 3s, then route to a hub landmark.
- **Passer wins:** disengage to two steps within 5s.
- **Rules:** any chase without first establishing clamp/contain = rep loss.
- **Reset:** 3s hold + landmark, or 5s escape.
- **Rounds:** 8 reps each, switch.