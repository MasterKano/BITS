PATH: SYS/Guard/Open-Guard/entries_hq_part-1_off-balance_to_thread-turn.md

# Entries (HQ) — Part 1: Off-Balance → Thread → Turn (HQ as a Controlled Entry, Not a Stalemate)

## 1. Purpose
Define HQ as an **entry bridge** (not a neutral pause): you use off-balancing to force a base event, then **thread** and **turn** into the correct side/line. This module sets the invariant that HQ progress must be built on:
- a base break (post/step/weight shift),
- a thread that captures the correct line,
- a turn that converts positional pressure into a leg-entry path (not getting pinned under pressure).

## 2. Inputs / Preconditions
- Opponent is in or near **HQ** (one leg between/near your legs; pressure potential present).
- You can maintain at least one barrier/anchor (frame or leg line control) to avoid flattening.
- You can create an off-balance event (pull/push/angle change) that forces a post or a step.
- You can recognize whether the opponent is trying to:
  - consolidate pressure (collapse), or
  - disengage/backstep (withdraw).

## 3. Outputs / Success Criteria
- You force a base event from HQ: post hands, widen, or step.
- You thread a controlling structure (leg line capture or wedge) that prevents one-step clear.
- You turn to the correct angle so HQ does not convert into a pin against you.
- You arrive at a stable downstream lane (HQ Parts 2–3, or hub selection) with escape denial.

## 4. Core Model / Engine
**HQ CONTACT → OFF-BALANCE (trigger) → THREAD (capture) → TURN (angle) → CONSOLIDATE → ROUTE**

Operational loop:
1) Identify the threat (collapse vs withdraw).
2) Create off-balance to force post/step.
3) Thread the capture (deny one-step clear).
4) Turn to a stable alignment (avoid being flattened).
5) Consolidate and route to the correct HQ continuation or hub.

## 5. Gates (override rules)

### 5.1 Hip Line Safety Gate (anti-flattening)
If HQ is collapsing you, entry attempts are suspended.
- **Default action:** frame high/low + turn-to-side + shrimp → rebuild barriers before threading.

### 5.2 Trigger Gate (off-balance first)
Threading without a base event leads to stalls and pressure conversion.
- **Default action:** off-balance until a post/step/weight shift appears; then thread.

### 5.3 One-Step Clear Gate (capture integrity)
If the leg can clear in a single step, your thread is not real.
- **Default action:** re-thread lower (ankle/knee line) and add redundancy before turning.

### 5.4 Turn Timing Gate (don’t turn under stable pressure)
Turning under stable pressure increases risk of being pinned.
- **Default action:** confirm off-balance or frame dominance before turning.

## 6. Top-6 Situations Playbook
1) **HQ pressure begins to collapse you**  
   → **Default:** safety first: frames + turn-to-side + shrimp; re-enter HQ contest.

2) **HQ is present but opponent is balanced/stable**  
   → **Default:** off-balance first; do not thread without trigger.

3) **Opponent posts hand(s) to stabilize**  
   → **Default:** trigger satisfied; thread immediately.

4) **Opponent takes a recovery step / weight shift**  
   → **Default:** thread the leg line; deny one-step clear.

5) **You threaded but opponent still steps free**  
   → **Default:** thread is too high/thin; re-thread lower and add redundancy.

6) **Opponent tries to withdraw/backstep from HQ**  
   → **Default:** treat as distance governance problem: capture integrity + follow foot.

## 7. Opponent Reactions → Responses
- **Drive/flatten from HQ:** abort entry; frame/angle; rebuild.
- **Post/widen/step:** thread now; capture becomes real.
- **Knee/leg clears in one step:** re-thread lower; add second control point.
- **Backstep:** follow foot; keep capture centered; do not freeze.

## 8. Failure Signatures → Fix
- **“I threaded and got smashed.”** → you violated Hip Line Safety or Turn Timing; frame and off-balance first.
- **“I can’t hold the capture.”** → one-step clear exists; thread lower and add redundancy.
- **“HQ feels like a stalemate.”** → you’re missing the Trigger Gate; force post/step before threading.

## 9. Trigger Recognition Checklist
Thread/turn only when 2+ cues are present:
- [ ] post hands
- [ ] widen base
- [ ] forced recovery step
- [ ] clear weight shift (hip line changes)
- [ ] opponent’s posture height changes (stack compromised)

## 10. Quality / Capture Checklist
- [ ] hip line is safe (no immediate flattening)
- [ ] a base event occurred before thread
- [ ] thread denies one-step clear
- [ ] turn is executed from advantage (not under stable pressure)
- [ ] you can route immediately to the next HQ continuation

## 11. Interfaces (routing rules)
- `entries_hq_part-2_backside_governance_follow-backstep.md` — use when: opponent’s primary HQ defense is backstep/withdraw and you must follow and govern backside.
- `entries_hq_part-3_consolidation_exit-traps_finish.md` — use when: you have a real capture and must consolidate into a finish/exit-trap sequence.
- `governance_anti-backstep.md` — use when: backstep is the dominant exit and distance governance decides success.
- `retention_framing_layer_frame-high-frame-low.md` — use when: HQ is collapsing into pressure and you must survive before threading.
- `application_cycle-break_to_immediate-counter.md` — use when: HQ entry occurs immediately after a cycle break.

## 12. Diagram
~~~
HQ ENTRY BRIDGE (off-balance -> thread -> turn)

[HQ contact]
    |
    v
[Threat ID: collapse vs withdraw]
    |
    +--> collapse -> frames/turn/shrimp -> rebuild
    |
    v
[OFF-BALANCE to force base event]
(post / step / widen / weight shift)
    |
    v
[THREAD capture]
(deny one-step clear)
    |
    v
[TURN to stable angle]
(no turn under stable pressure)
    |
    v
[CONSOLIDATE -> ROUTE]
(HQ part 2 / part 3 / hub)
~~~

## 13. Drills and Games

### 13.1 Trigger-First Threading
- **Start:** opponent establishes HQ contact; begins stable.
- **Defender wins:** create a base event (post/step/widen), then thread capture and pause 2s.
- **Passer wins:** deny base event for 10s or flatten/pin 3s.
- **Rules:** any thread attempt before base event = rep loss.
- **Reset:** 2s pause or 10s/pin.
- **Rounds:** 8 reps each, switch.

### 13.2 One-Step Clear Audit
- **Start:** defender has a “thread”; opponent’s only job is to clear in one step if possible.
- **Defender wins:** deny one-step clear for 5s (capture integrity).
- **Passer wins:** one-step clear within 5s.
- **Rules:** defender must fix by re-threading lower and adding redundancy (no hand chasing).
- **Reset:** 5s hold or clear.
- **Rounds:** 8 reps each, switch.

### 13.3 Turn Timing Under Pressure
- **Start:** HQ contact; opponent alternates between stable pressure and post/step cues.
- **Defender wins:** only turn on trigger; avoid being flattened for 10s.
- **Passer wins:** flatten/pin 3s after a premature turn.
- **Rules:** premature turn = immediate rep loss.
- **Reset:** 10s survive or 3s pin.
- **Rounds:** 6 reps each, switch.