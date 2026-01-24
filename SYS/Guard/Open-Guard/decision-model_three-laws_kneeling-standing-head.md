PATH: SYS/Guard/Open-Guard/decision-model_three-laws_kneeling-standing-head.md

# Decision Model — Three Laws (Kneeling / Standing / Head Height)

## 1. Purpose
A decision model that selects the correct Open Guard response family by reading three high-leverage context signals:

1) **Kneeling vs Standing** (base geometry and likely pass-building route)  
2) **Head height** (attack lane availability: legs vs go-behind)  
3) **Resulting risk** (hip line threat vs reset threat)

Goal: reduce decision latency and prevent wrong-family actions (e.g., treating kneeling as harmless, chasing grips while the opponent backsteps, entering under stable posture).

## 2. Inputs / Preconditions
- You can see the opponent’s base state (kneeling or standing).
- You can track head height relative to your hip line and their hips.
- You can maintain or restore orientation (feet or knees facing).

## 3. Outputs / Success Criteria
Correct application yields at least one within 5–10 seconds:
- **Keep in front:** no outside knee line progression.
- **Deny the next chain link:** level/penetration stopped early.
- **Earn a base event:** post/widen/forced step.
- **No free reset:** opponent cannot disengage to two steps.
- **Cycle break → counter:** if hip line threatened, recovery is followed immediately by offense.

## 4. Core Model / Engine

### 4.1 The Three Laws (executable)
**Law 1 — Kneeling is not neutral**  
Kneeling often means: shorter distance to pressure, easier level change, and direct lines to your hips.

- If kneeling + forward intent: treat as **forward+push** until proven otherwise.
- Default: structure earlier; protect hip line; deny level and shoulder line.

**Law 2 — Standing amplifies reset threat**  
Standing makes disengage/backstep easier and makes circling outside knee line cheaper.

- If standing + backward intent: treat as **backward+pull** until proven otherwise.
- Default: anti-exit governance; follow with hips; upgrade to true handle.

**Law 3 — Head height selects the lane**
- **Head high:** leg lane is open; persistent leg-line threats slow passing.
- **Head low:** go-behind / upper-body routes become available; punish head position.
- Head changes quickly; re-read continuously, but do not violate gates.

### 4.2 Domain Progression Chain Hooks (what each context tends to build)
- **Kneeling + forward:** threatens **Level → Penetration → Pin**
- **Standing + circle:** threatens **Angle** (outside knee line) then **Penetration**
- **Standing + retreat:** threatens **Reset/Disengage**
- **Head low during engagement:** grants access to **go-behind** style counters (if cycle break exists)

### 4.3 Routing Heuristics (fast defaults)
- **Kneeling + close:** frames first, turn-to-side early, shrimp only after structure is set.
- **Standing + far:** connect to ankle/heel line; keep them in front; don’t accept reset.
- **Head high:** legs first (ankle line, shin-to-shin, distance breakers).
- **Head low:** punish with go-behind or upper-body routing, but only after cycle break / stability.

## 5. Gates (override rules)

### 5.1 Hip Line Gate
If hip line is threatened: defensive cycle until cycle break.

**Default action:** frames high/low → turn-to-side → shrimp/recover barriers → re-square.

### 5.2 Hands-Down Gate
No committed entries/rotations under stable base.

**Default action:** off-balance until post/widen/forced step occurs → then commit.

### 5.3 Orientation Rule
Feet or knees must face opponent continuously.

**Default action:** re-square hips + reinsert barriers before attempting upgrades.

## 6. Opponent Reactions → Responses (Context Matrix)

### 6.1 Kneeling (primary risk: pressure)
- **Kneeling + forward drive:** structure early; protect hip line; deny level.
- **Kneeling + stall then burst:** keep barriers active; treat burst as forward+push.
- **Kneeling + grip strip:** reattach leg line; re-square; don’t reach.

### 6.2 Standing (primary risk: angle + reset)
- **Standing + circle:** foot pummel + crossover/scoot; keep them in front.
- **Standing + backstep:** follow immediately; upgrade to true handle (ankle/heel line).
- **Standing + shove-to-clear:** reinsertion first; then re-center; attach ankle.

### 6.3 Head height (lane selector)
- **Head high:** threaten leg line constantly; use distance-based connectors.
- **Head low:** threaten go-behind/upper-body counters when available; do not chase if it breaks orientation.

## 7. Failure Signatures → Fix
- **“Kneeling felt safe, then I got smashed”** → violated Law 1; treat kneeling forward intent as pressure; structure earlier.
- **“He just reset and I lost everything”** → violated Law 2; standing increases reset; follow with hips and build true handle.
- **“I chased head low and lost angle/orientation”** → chased lane without gates; re-square first; punish head low only when stable.
- **“I entered under stable posture”** → hands-down gate violated; base-break longer.
- **“I kept losing outside knee line”** → failed standing-circle response; foot reinsertion + crossover/scoot sooner.

## 8. Interfaces (use-when tags)
- `open-guard_master-operating-system.md` — use when: running the full controller loop and routing.
- `decision-model_dynamic-energy-theory.md` — use when: mapping push/pull + forward/back into the response family.
- `counter-offense_golden-rule_head-height.md` — use when: selecting leg attacks vs go-behind based on head height.
- `retention_framing_layer_frame-high-frame-low.md` — use when: kneeling/pressure requires structure.
- `retention_movement_foot-pummeling.md` — use when: standing/circle or shove-to-clear threatens barriers.
- `retention_movement_crossovers.md` — use when: outside knee line is forming; hips must re-square.
- `retention_movement_scooting.md` — use when: you must follow retreats while staying squared.
- `entries_distance_2-on-1-ankle-system.md` — use when: head high + distance exists; secure ankle line early.
- `entries_distance_shin-to-shin_connector.md` — use when: mid-range entry connection is required.
- `entries_kneeling_single-leg-entry.md` — use when: kneeling base exposes a reachable leg under compromised posture.

## 9. Diagram (ASCII)

~~~
THREE LAWS (Open Guard)

LAW 1: KNEELING ≠ NEUTRAL  -> primary risk = PRESSURE (Level->Penetration->Pin) -> STRUCTURE EARLY
LAW 2: STANDING amplifies RESET/ANGLE -> primary risk = OUTSIDE KNEE LINE + BACKSTEP -> FOLLOW + TRUE HANDLE
LAW 3: HEAD HEIGHT selects LANE
   head high -> LEG LANE (ankle/heel line, distance connectors)
   head low  -> GO-BEHIND/UPPER routes (when stable; do not chase)

GATES OVERRIDE:
HIP LINE -> DEFENSIVE CYCLE
NO HANDS-DOWN -> NO COMMITTED ENTRY
ORIENTATION -> INVARIANT
~~~

## 10. Drills and Games (Game Cards)

### 10.1 Kneeling Pressure Gate
- **Start:** passer kneeling in front; defender open guard.
- **Defender wins:** avoid hip line threat and keep opponent in front for **20s**.
- **Passer wins:** **hip line touch** or **pin**.
- **Rules:** passer must drive forward (no retreats); defender must use structure early (frames/turn/shrimp).
- **Reset:** hip line touch / pin / timer.
- **Rounds:** 8×20s, switch.

### 10.2 Standing Reset Denial
- **Start:** passer standing at range; light contact allowed.
- **Defender wins:** prevent **disengage to two steps** for **15s** while maintaining any contact.
- **Passer wins:** **disengage to two steps** with no contact.
- **Rules:** passer must attempt backstep/retreat frequently; defender must follow with hips and upgrade to ankle/heel line.
- **Reset:** disengage / timer.
- **Rounds:** 8×20s, switch.

### 10.3 Head-Height Lane Selection
- **Start:** passer standing; defender seated open guard.
- **Defender wins:** when head stays high: secure ankle/heel line and keep in front **3s**; when head goes low: initiate go-behind style counter and keep in front **3s**.
- **Passer wins:** **outside knee line** then **hip line touch** or **pin**.
- **Rules:** passer alternates head height naturally (posture changes are allowed); defender must take the correct lane without breaking orientation.
- **Reset:** 3s hold / hip line touch / pin.
- **Rounds:** 8×20s, switch.