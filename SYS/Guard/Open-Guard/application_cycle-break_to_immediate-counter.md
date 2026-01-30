PATH: SYS/Guard/Open-Guard/application_cycle-break_to_immediate-counter.md

# Application — Cycle Break → Immediate Counter (No Stop-Pass-Stop)

## 1. Purpose
A mandatory application rule that prevents “recover guard then pause.”

Rule: **every cycle break must immediately convert into counter-offense**.

This is the glue between defence (retention) and offence (entries/counters). It makes recovery meaningful and prevents the passer from resetting safely.

## 2. Inputs / Preconditions
- You enter a defensive cycle because of hip line threat or severe angle.
- You have the ability to re-center and rebuild barriers (legs/frames).
- You can start at least one counter lane (leg lane or go-behind) without losing orientation.

## 3. Outputs / Success Criteria
A successful rep produces, within 2 seconds of cycle break:
- a **counter start** (Section 4.2), and then
- either (a) sustained contact that prevents reset, or (b) an entry attempt that forces a base event.

Failure is defined as:
- cycle break achieved, followed by hesitation/reset acceptance.

## 4. Core Model / Engine

### 4.1 Cycle Break (operational definition)
Cycle break exists only when all are true:
- opponent is **in front** (no dominant outside knee line),
- **barriers** are rebuilt (legs/frames between bodies),
- **orientation** restored (feet or knees facing),
- hip line threat is removed (no immediate penetration line).

If any element is missing, you are still defending.

### 4.2 Immediate Counter Rule (timing)
- **Start a counter within 2 seconds** of cycle break.
- “Start” is about initiation, not completion.

### 4.3 What counts as a counter start (taxonomy)
A counter start is any one of these (choose the lowest complexity available):

**Leg lane starts (head high)**
- secure **ankle/heel line** (true handle), or
- establish shin-to-shin / leg-line connection that forces a reaction, or
- force post/widen/forced step via leg-line threat.

**Go-behind / upper-body starts (head low)**
- occupy space behind head/shoulders and begin circling to rear angle, or
- force head to turn away and take angle (while keeping orientation).

**Universal start**
- any action that prevents reset *and* initiates a new threat immediately.

## 5. Gates (override rules)

### 5.1 Hip Line Gate (safety first)
No counter until hip line threat is removed.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square → cycle break check.

### 5.2 Hands-Down Gate (commitment validity)
No committed rotations/entries under stable base.

**Default action:** base-break until post/widen/forced step occurs, then commit.

### 5.3 Orientation Rule
Counter starts must not violate facing.

**Default action:** re-square hips first; then start the counter.

## 6. Opponent Reactions → Responses (after counter start)
The passer’s best immediate defences against your counter start:

1) **Retreat / backstep reset**
   - Response: keep true handle; follow with hips; add redundancy.

2) **Drive back into pressure**
   - Response: keep barriers active; deny level; re-center; reselect counter on cycle break.

3) **Circle to outside knee line**
   - Response: crossover/scoot; keep opponent in front; foot reinsertion first.

4) **Strip grips immediately**
   - Response: reattach leg line (ankle/heel); do not reach; rebuild redundancy.

## 7. Failure Signatures → Fix
- **Cycle break but I paused** → enforce the 2-second rule; use a simplest start (ankle line).
- **Counter start breaks orientation** → choose leg lane first; re-square before switching lanes.
- **Counter start is too complex** → downgrade: attach ankle line and follow.
- **I countered but he reset anyway** → handle was thin; upgrade to true handle + redundancy.
- **I chased a finish and got passed** → violated gate; prioritize preventing reset first.

## 8. Interfaces (use-when tags)
- `open-guard_master-operating-system.md` — use when: enforcing the master loop (defense → cycle break → counter).
- `counter-offense_golden-rule_head-height.md` — use when: selecting leg lane vs go-behind at counter time.
- `decision-model_dynamic-energy-theory.md` — use when: opponent’s retreat/pressure changes which counter start is safest.
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: counter attempts risk losing facing.
- `entries_distance_2-on-1-ankle-system.md` — use when: selecting the simplest leg-lane counter start.
- `entries_distance_shin-to-shin_connector.md` — use when: mid-range leg-lane connection is the best start.

## 9. Diagram (ASCII)

~~~
DEFENSIVE CYCLE -> CYCLE BREAK CHECK -> (within 2s) COUNTER START

CYCLE BREAK requires:
- opponent in front
- barriers rebuilt
- orientation restored
- hip line threat removed

COUNTER START options:
- head high -> ankle/heel line true handle (simplest)
- head low  -> go-behind / rear-angle initiation (if stable)
- always -> prevent reset while starting threat

FAILURE = stop-pass-stop (cycle break then pause)
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Two-Second Rule (core)
- **Start:** passer mid-pass attempt; defender must recover.
- **Defender wins:** achieve cycle break then begin a counter within **2s** (any valid counter start).
- **Passer wins:** **pin** or **disengage to two steps** after defender recovers.
- **Rules:** if defender pauses after cycle break, rep is a loss.
- **Reset:** counter start / pin / disengage.
- **Rounds:** 12 reps each, switch.

### 10.2 Simplest Start Only (ankle line)
- **Start:** defender begins at cycle break state; passer standing in front.
- **Defender wins:** secure ankle/heel line (true handle) and prevent disengage for **15s**.
- **Passer wins:** **disengage to two steps** or achieve **outside knee line** then **hip line touch**.
- **Rules:** defender may not attempt any other entry until ankle/heel line is secured.
- **Reset:** timer / disengage / hip line touch.
- **Rounds:** 8×20s, switch.

### 10.3 Counter or Re-Defend (pressure return)
- **Start:** defender at cycle break; passer must immediately drive forward.
- **Defender wins:** start counter within **2s** OR re-enter defensive cycle correctly and return to cycle break within the round.
- **Passer wins:** **pin** or flattened shoulders **3s**.
- **Rules:** passer’s only goal is forward pressure; defender must demonstrate correct phase switching.
- **Reset:** pin / 3s hold / cycle break + counter start.
- **Rounds:** 8×20s, switch.

### 10.4 Prevent the Reset (retreat specialization)
- **Start:** cycle break achieved; passer tries to backstep/retreat immediately.
- **Defender wins:** maintain any contact for **15s** and show at least one counter start.
- **Passer wins:** **disengage to two steps**.
- **Rules:** defender must follow with hips; “hand chasing” is penalized by restart.
- **Reset:** timer / disengage.
- **Rounds:** 8×20s, switch.