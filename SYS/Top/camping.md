# Camping

## Purpose

A top stabilization hub used to:
- stop re-guarding after leg exchanges / denied backtakes,
- force predictable turning reactions,
- restart the pass/back conversion loop without resetting to neutral.

## Core idea

- Camping is a **control-and-fork** platform:
  - first you satisfy control gates (hip line + cranial shift),
  - then you force a fork:
    - turn-toward → pin/pass
    - turn-away → back attachment
    - turtle → tight waist connector
- Camping is also the default “catch” after denied transitions: you land here to avoid scrambles.

## ASCII system diagram

~~~text
(leg exit / denied backtake / failed ride) -> [Camping]
                         |
                         v
               +------------------+
               | CONTROL GATES    |
               | - hip line pinned|
               | - knees denied   |
               | - cranial shift  |
               | - no clean rise  |
               +--------+---------+
                        |
                        v
                 {REACTION FORK}
        +-----------+-----+--------------+
        |                 |              |
   turn toward         turn away       turtle
   (faces)             (runs)          (folds)
        |                 |              |
        v                 v              v
 [Pin/Pass lane]     [Back lane]     [Tight waist]
 (stay chest2chest) (connect first)  (flatten / branch)
        |
        v
(if denied/slips) -> [Stabilizer hierarchy]
  1) stay in Camping + re-force turn
  2) North-south (if forward step + cranial control)
  3) Cross-body ride (if roll/angle required)
~~~

## Key positions

- Outside camping (primary hub)
  - Hip line pinned so they cannot freely re-guard.
  - Knees are managed so they cannot point knees back into you to square.
  - Cranial shift prevents free head/shoulder rotation.
- Camping as “midpoint control”
  - You are not committed to a specific pass yet; you are committed to forcing a reaction.
- Camping as “denied attempt catch”
  - When hooks/ride/backtake attempts slip, camping is the landing that preserves advantage.

## Entries

- Denied backtake (hooks or attachment slipping)
  - Immediate drop to camping rather than chasing hooks from distance.
- Leg entanglement exit (knee line cleared / legs separated)
  - Enter camping to prevent re-square and re-lock.
- Failed ride / failed roll entry
  - If cross-body ride attempt does not stabilize, land in camping and re-run gates.
- Anti-stand/heist catch
  - If they begin building height, camping is the hip-line clamp that forces them back down.

## Key cues (operational)

- “If their knees point into me, I am not camping.”
- “If I’m past legs but can’t progress, I’m missing cranial shift.”
- “I don’t chase outcomes from camping; I force turns.”
- “Denied backtake = not a reset; it is a trigger to camp.”

## Control gates (must be true before you branch)

### 1) Hip line pinned
- Their hips cannot freely slide away from your pressure.
- Their hips are not drifting under you into re-guard space.

### 2) Knees denied (anti re-guard)
- They cannot point knees back into you to square.
- If their knees are returning inside, you re-angle before advancing.

### 3) Cranial shift present
- Their head/shoulders cannot freely rotate to re-square.
- If cranial control is missing, you cannot reliably force the fork.

### 4) No clean rise
- They cannot build a stable base to stand/heist without you collapsing it.
- If they are coming up, you re-camp hips first, then progress.

## Decision rules (IF/THEN) — lane-by-lane

### A) Establishment (getting camping stable)
- IF you land in camping after a denied attempt -> THEN freeze hip line first, then add cranial shift.
- IF they are re-guarding by bringing knees back in -> THEN re-angle and re-pin hips before chasing progress.
- IF you are “past legs” but can’t progress -> THEN treat it as cranial shift failure; fix head/shoulders first.

### B) Reaction forcing (creating the fork)
- IF camping is stable but no reaction occurs -> THEN increase cranial pressure to force a turn (do not chase legs).
- IF they rotate under you without committing to a turn -> THEN you lack cranial shift or hip pin; re-satisfy gates.

### C) Branch: turn-toward (faces you)
- IF they turn toward -> THEN accept chest-to-chest and start pass progression immediately.
- IF they frame and re-square on turn-toward -> THEN re-win cranial shift before stepping deeper (do not drive into frames).
- IF they turn toward to stop the back -> THEN treat it as success; take the pin/pass.

### D) Branch: turn-away (runs)
- IF they turn away -> THEN attach chest-to-upper-back first (connection before hooks).
- IF you are too far to attach -> THEN close distance by upgrading upper-body control (do not reach for hooks).
- IF they run to turtle/quadpod as you attach -> THEN switch to tight waist (turtle trigger).

### E) Branch: turtle (folds)
- IF turtle forms -> THEN tight waist is the stabilizer; flatten or run back/pass branches from there.
- IF turtle is unstable and they may stand -> THEN keep hip line pinned and collapse height before hook chasing.

### F) Stabilizer hierarchy (when camping isn’t holding)
- IF camping is stable -> THEN stay and re-force the fork (default).
- IF forward step is available and head line is controlled -> THEN transition to north-south.
- IF you need roll/angle to stay connected (they’re turning/rolling) -> THEN transition to cross-body ride.
- IF denied back lane but turtle is forming -> THEN tight waist.

## Opponent counters + immediate answers

- Counter: re-guard by inserting knees back toward you.
  - Answer: re-angle + re-pin hips; do not chase head while knees are inside.
- Counter: rotate shoulders to re-square while hips stay pinned.
  - Answer: cranial shift upgrade; head/shoulder control before advancing.
- Counter: build height (stand/heist) to escape pressure.
  - Answer: re-camp hips, collapse base, then re-run fork.
- Counter: turn-away sprint (distance creation).
  - Answer: close distance to upper back first; hooks are downstream.

## Failure signatures + fixes (fast diagnostics)

- “I’m in camping but nothing is happening.”
  - You are missing cranial shift or hip pin; re-run gates before branching.
- “They keep getting knees back in.”
  - Your knee/hip angle is wrong; fix knee denial first.
- “I chase hooks and they re-face.”
  - You skipped upper-back connection; connect first, then hook.
- “Denied backtake becomes a scramble.”
  - You failed to land in camping immediately; treat denial as the trigger to camp.

## Completion checks

- You can hold them in a state where:
  - knees cannot point back into you,
  - head/shoulders cannot freely rotate,
  - and a clean stand/heist is denied.
- You can force one of:
  - turn-toward (pass start),
  - turn-away (back attachment start),
  - turtle (tight waist trigger),
  without resetting to neutral.

## Links

- `../meta/conversion-loop.md`
- `../meta/cranial-shift.md`
- `../meta/back-completion-criteria.md`

## Sources

- Gordon Ryan — Pillars of Defense: Leg Locks to Back Takes
  - `INS/gr-pod/VN/v2.md`
  - `INS/gr-pod/VN/v4.md`
  - `INS/gr-pod/VN/v5.md`
