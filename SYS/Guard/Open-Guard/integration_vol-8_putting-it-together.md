PATH: SYS/Guard/Open-Guard/integration_vol-8_putting-it-together.md

# Integration (Vol 8) — Putting It Together (Routing, Selection, and Non-Drift Assembly)

## 1. Purpose
This is the integration controller for Vol 8: it defines how the open guard system is **assembled and routed** in real time without drifting into random technique selection.

Core invariants:
- **Retention first** (deny passing progress before attacking).
- **Entry selection is contextual** (kneeling vs standing, pressure vs mobility, head height).
- **Every exchange must route**: retention → entry family → hub → stabilization → finish, or reset to retention.

## 2. Inputs / Preconditions
- You are in open guard and opponent is either:
  - kneeling/low (kneeling passer), or
  - standing (standing passer), or
  - transitioning between the two.
- You can maintain at least one barrier and can identify:
  - head height (high/low),
  - passer archetype (pressure vs mobility),
  - and the dominant escape pattern (backstep vs pull-away).

## 3. Outputs / Success Criteria
- You can identify the correct module family (distance / kneeling / RDLR / HQ / DLR / closed-guard bridge).
- You can avoid “dead ends” (stall positions) by using:
  - cycle-break to immediate counter,
  - anti-backstep governance,
  - anti-flee governance,
  - and hub selection rules.
- You can re-enter retention rapidly when threatened.

## 4. Core Model / Engine (Routing Spine)
**RETENTION → THREAT ID → ENTRY FAMILY → HUB → STABILIZE → FINISH / RESET**

### 4.1 Threat Identification (fast classifier)
- **Collapse threat:** pressure consolidation, head low/drive, chest-to-chest intent.
- **Withdraw threat:** backstep, pull-away/disengage, stance reset.
- **Neutral threat:** probing/feints; no committed collapse or withdraw yet.

### 4.2 Entry Family Selection (by opponent state)
- **Kneeling passer:** use kneeling entries (single/double/reverse-double/cross-catch/hip-pin).
- **Standing passer:** use distance entries (2-on-1 ankle, shin-to-shin) and stance-based hooks (RDLR/DLR).
- **HQ appears:** run HQ bridge (off-balance → thread → turn; follow backstep; consolidate).
- **RDLR appears (pressure drives you flat):** run RDLR platform; convert to containment; deny pinch/pack defenses.
- **DLR appears (outside hook opportunity):** enforce no-gi attachment rules; migrate outside-to-inside.
- **Closed guard opportunity appears:** only if two-leg control requirement is satisfied; then bridge to X on open.

## 5. Gates (override rules)

### 5.1 Retention Gate (non-negotiable)
If hip line is threatened or you are being flattened, entry selection is suspended.
- **Default action:** frames high/low + turn-to-side + shrimp → rebuild barriers.

### 5.2 Head Height Gate (golden rule compliance)
Your counter-offense must respect head height (do not choose entries that lose you head height governance).
- **Default action:** if opponent’s head is low and driving, treat as collapse threat and prioritize retention/cycle-break before entries.

### 5.3 Anti-Backstep Gate (dominant universal escape)
When backstep is present, route to governance first.
- **Default action:** foot to center line; follow foot; re-thread lower; re-lock.

### 5.4 Anti-Flee Gate (pull-away)
When pull-away/disengage begins, lock or route.
- **Default action:** clamp/contain if possible; if contact breaks, route to distance re-capture.

### 5.5 No Dead-End Gate
If you cannot progress for 3–5 seconds, you must switch family (do not stall).
- **Default action:** apply cycle-break → immediate counter OR switch to an adjacent entry family.

## 6. Top-6 Situations Playbook (integration-level)
1) **You feel pass progression building**  
   → **Default:** retention first; deny six-elements-of-passing progress; then re-enter.

2) **Opponent is kneeling and stable**  
   → **Default:** create trigger (post/step/widen), then kneeling entry (single/double/reverse-double).

3) **Opponent is standing and mobile**  
   → **Default:** distance entries (2-on-1 ankle / shin-to-shin); threaten legs constantly.

4) **Opponent drives you flat / pressure collapses**  
   → **Default:** RDLR platform; hands-to-mat base-break; deny pinch/pack defense; route to hub.

5) **HQ contact appears + opponent backsteps**  
   → **Default:** follow foot; center-line distance governance; re-thread and consolidate.

6) **Closed guard becomes available (two-leg control)**  
   → **Default:** close legally; when they open, bridge immediately to X.

## 7. Opponent Reactions → Responses (integration routing)
- **Collapse (pressure):** retention → framing layer → cycle-break → re-attack.
- **Withdraw (backstep):** anti-backstep governance → follow → re-lock.
- **Withdraw (pull-away):** clamp or route to distance connectors.
- **Knee pinch/pack (blocks pummels):** clear pinch/pack or switch family.
- **Stance reset:** distance re-capture; re-enter using shin-to-shin or 2-on-1 ankle.

## 8. Key Cues (integration-level)

### 8.1 Family Selection Cues (triggers)
- **Kneeling trigger:** hands post / widen base / forced step / head height change.
- **Standing trigger:** leg becomes “available” (step forward), ankle line reachable, stance stagger appears.
- **RDLR trigger:** forward drive flattens you; near leg heavy and close; calf access appears.
- **HQ trigger:** leg threads between your legs; pressure potential present.
- **DLR trigger:** outside hook opportunity + true handle available.
- **Closed guard trigger:** two-leg control already established (permission cue).

### 8.2 Abort Cues (reset to retention)
- shoulders pinned + chest-to-chest pressure building,
- hips pinned and angle cannot be recovered,
- you lose both anchors (no control points),
- you are chasing a moving target without distance governance.

### 8.3 Success Landmarks (you are “in system”)
- you can deny one-step clear,
- you have a clear route to a hub within one action,
- backstep/pull-away are already governed,
- you can hold the state for 3 seconds without scrambling.

## 9. Failure Signatures → Fix
- **Random technique drift** → enforce routing spine; name the family before acting.
- **Stalling in half-positions** → apply No Dead-End Gate; switch families.
- **Losing to backstep repeatedly** → treat anti-backstep as primary; govern distance first.
- **Losing to pull-away repeatedly** → clamp earlier or accept route-to-distance without chasing.
- **Getting flattened mid-entry** → retention gate violated; frames first.

## 10. Interfaces (routing rules)
- `open-guard_master-operating-system.md` — use when: you need the global operating priorities and selection structure.
- `application_cycle-break_to_immediate-counter.md` — use when: you break a passing cycle and must counter without pause.
- `retention_model_knowledge-denial.md` — use when: you must deny the passer knowing the next link.
- `retention_model_six-elements-of-passing.md` — use when: diagnosing passer progress and selecting denial action.
- `counter-offense_golden-rule_head-height.md` — use when: head height governs safe counter-offense.
- `application_mobility-passer_defense-loop.md` — use when: mobility passer requires looping defense logic.
- `application_pressure-passer_defense-ladder.md` — use when: pressure passer requires ladder defense logic.
- `entries_distance_2-on-1-ankle-system.md` — use when: standing distance capture is the best re-entry.
- `entries_distance_shin-to-shin_connector.md` — use when: mid-range anchoring is required for re-entry.
- `entries_kneeling_single-leg-entry.md` — use when: kneeling passer exposes one leg cleanly.
- `entries_kneeling_double-leg-entry_half-sumi-trigger.md` — use when: kneeling passer base-break creates double entry permission.
- `entries_rdrl_part-1_base-break-platform.md` — use when: pressure collapses you and RDLR platform is available.
- `entries_hq_part-1_off-balance_to_thread-turn.md` — use when: HQ contact appears and you must treat it as an entry bridge.
- `entries_dlr_part-1_no-gi_attachment_rules.md` — use when: outside hook appears and you must attach correctly in no-gi.
- `entries_closed-guard_part-1_two-leg-control_requirement.md` — use when: considering closure; permission rules apply.
- `entries_closed-guard_part-2_closed-to-x-guard_bridge.md` — use when: they open; you convert to X.

## 11. Diagram
~~~
OPEN GUARD INTEGRATION ROUTER (Vol 8)

           [RETENTION]
                |
                v
        [THREAT IDENTIFY]
   collapse / withdraw / neutral
        |         |         |
        v         v         v
   (collapse)  (withdraw)  (neutral)
   frames+     backstep:   pick family by
   cycle-break center-line  kneeling/standing
        |      follow foot      |
        v         |             v
 [ENTRY FAMILY SELECT] <---------+
  kneeling | distance | RDLR | HQ | DLR | closed
        |
        v
       [HUB]
 (double 50 / 50-50 / criss-cross / inside senkaku)
        |
        v
 [STABILIZE 3s + EXIT TRAPS]
 backstep governed / pull-away denied
        |
        v
 [FINISH] or [RESET -> RETENTION]
~~~

## 12. Drills and Games

### 12.1 Name-the-Family Routing Game (anti-drift)
- **Start:** open guard; partner alternates kneeling/standing entries each rep.
- **Defender wins:** correctly name the family (distance/kneeling/RDLR/HQ/DLR/closed) and reach a stable landmark (deny one-step clear) within 10s.
- **Passer wins:** force flatten/pin 3s or disengage to two steps.
- **Rules:** acting without naming the family = rep loss.
- **Reset:** landmark, pin, or disengage.
- **Rounds:** 12 reps each, switch.

### 12.2 Backstep vs Pull-Away Branching
- **Start:** partner chooses either backstep or pull-away as primary defense on cue.
- **Defender wins:** apply correct branch: backstep -> center-line follow; pull-away -> clamp or distance route; hold 3s.
- **Passer wins:** complete escape within 5s.
- **Rules:** wrong branch choice = rep loss.
- **Reset:** 3s hold or escape.
- **Rounds:** 10 reps each, switch.

### 12.3 No Dead-End Timer (switch families)
- **Start:** defender begins in any entry family; partner resists but does not fully escape.
- **Defender wins:** if no progress in 5s, execute a correct family switch and reach a new landmark within 10s.
- **Passer wins:** defender stalls >5s without switching, or passer pins 3s / disengages.
- **Rules:** “stall without switch” is the fail condition.
- **Reset:** landmark, stall fail, pin, or disengage.
- **Rounds:** 8 reps each, switch.