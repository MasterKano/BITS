PATH: SYS/Guard/Open-Guard/retention_movement_scooting.md

# Retention Movement — Scooting (Follow + Re-Center)

## 1. Purpose
A retention movement system for **following** a passer who retreats, backsteps, or circles away while keeping them **in front**.

Scooting is the “anti-exit locomotion” that prevents:
- clean disengage to two steps,
- angle creation through lateral runaround,
- you losing contact while attempting to reattach.

## 2. Inputs / Preconditions
- You can move hips on the mat without standing.
- You can keep at least one contact point (hand or foot) while moving.
- You can re-square hips continuously (orientation invariant).

## 3. Outputs / Success Criteria
- You stay connected through the passer’s retreat/backstep.
- Passer cannot disengage to two steps.
- You keep opponent in front (outside knee line denied).
- You can upgrade to ankle/heel line true handle during or after the follow.

## 4. Core Model / Engine

### 4.1 What Scooting Does
- Moves your hips to match the passer’s exit path.
- Maintains orientation while distance changes.
- Preserves the ability to reinsert barriers and/or attach leg line.

### 4.2 Triggers (when to scoot)
Scooting is triggered by:
- backstep or step-away attempts,
- circling away after shove-to-clear,
- any “reset attempt” where your reaction must be immediate.

If the passer is driving forward into pressure, scooting becomes secondary to structure (frame stack).

### 4.3 Domain Progression Chain Hooks
Scooting primarily denies:
- **Reset/Disengage** and also reduces
- **Angle** by keeping the opponent centered as distance changes.

## 5. Gates (override rules)

### 5.1 Orientation Rule (primary)
Feet or knees face opponent while scooting.

**Default action:** re-square each beat as you follow; do not scoot sideways while turned away.

### 5.2 Hip Line Gate
If hip line is threatened during the follow (they turn exit into pressure), switch to defensive cycle.

**Default action:** frames high/low → turn-to-side → shrimp → rebuild → re-square.

### 5.3 Hands-Down Gate (commitment)
Scooting is follow/deny reset; it is not a reason to commit to entries under stable base.

**Default action:** follow first; attach ankle/heel line; commit only after base event.

## 6. Opponent Reactions → Responses

1) **Backstep reset**
   - Response: scoot immediately; keep connection; upgrade to ankle/heel line; add redundancy.

2) **Hard retreat (two-step attempt)**
   - Response: scoot with hips; keep any contact; deny the second step by attachment.

3) **Retreat then circle**
   - Response: scoot to keep centered; crossover if outside knee line starts forming.

4) **Retreat turns into forward pressure**
   - Response: switch to frame stack; treat as forward+push; defensive cycle if hip line threatened.

## 7. Failure Signatures → Fix
- **He gets two steps away** → follow latency; scoot earlier; prioritize contact over “better grips.”
- **I scoot but get angled** → hips are following but not squaring; add crossover re-square each beat.
- **I keep losing contact** → thin handle; upgrade to ankle/heel line; add redundancy (hand+foot).
- **I scoot into pressure and get crushed** → misread; pressure requires frames first.

## 8. Interfaces (use-when tags)
- `decision-model_dynamic-energy-theory.md` — use when: backward+pull (reset) is identified.
- `application_mobility-passer_defense-loop.md` — use when: retreat/backstep is the passer’s main defense.
- `retention_movement_crossovers.md` — use when: following turns into outside knee line threat.
- `entries_distance_2-on-1-ankle-system.md` — use when: scooting creates ankle-line attachment window.
- `retention_orientation_rule_feet-or-knees-facing.md` — use when: following must maintain facing.
- `retention_framing_layer_frame-high-frame-low.md` — use when: retreat turns into pressure and structure is needed.

## 9. Diagram

~~~
SCOOTING = FOLLOW + RE-CENTER

trigger: backstep / retreat / reset attempt
action: hips travel immediately while facing -> keep contact -> deny "two steps"
upgrade: ankle/heel true handle + redundancy
if following creates angle -> add CROSSOVER
if retreat turns into pressure -> FRAME STACK / DEFENSIVE CYCLE
~~~

## 10. Drills and Games (Game Cards)

### 10.1 No Two Steps (anti-reset)
- **Start:** range with light contact allowed.
- **Defender wins:** prevent **disengage to two steps** for **15s** while maintaining any contact.
- **Passer wins:** **disengage to two steps** with no contact.
- **Rules:** passer must attempt hard retreats/backsteps repeatedly; defender must scoot immediately (hips travel).
- **Reset:** disengage / timer.
- **Rounds:** 8×20s, switch.

### 10.2 Backstep Follow → True Handle
- **Start:** passer initiates backstep; defender begins seated open guard.
- **Defender wins:** scoot to follow and secure ankle/heel line (true handle) within **5s**.
- **Passer wins:** strips contact then disengages to two steps.
- **Rules:** defender must follow first, then upgrade (no reaching while stationary).
- **Reset:** true handle / disengage.
- **Rounds:** 10 reps each, switch.

### 10.3 Follow Creates Angle (follow + re-square)
- **Start:** passer retreats and circles immediately.
- **Defender wins:** scoot to follow and re-square (deny outside knee line), then hold “in front” for **3s**.
- **Passer wins:** **outside knee line** for **3s** or **hip line touch**.
- **Rules:** defender must demonstrate scoot + crossover sequencing when needed.
- **Reset:** 3s hold / hip line touch.
- **Rounds:** 8×20s, switch.