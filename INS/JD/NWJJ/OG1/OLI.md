<!-- ================================================================ -->
<!-- Operator Library Index — Systems Only                                   -->
<!-- Single-file, anchor-stable, GitHub-ready                          -->
<!-- ================================================================ -->

# Operator Library — Systems Only

## How to use this library (fast)
**Default loop:** Context → Connect → Deny → Recenter → Convert → Stabilize → Anti-exit  
**When lost (3-card reset):** [A-04 Active Link](#a-04) → [A-06 Hip-Line Alarm](#a-06) → [C-09 Sequencing](#c-09)  
**Core rule:** No “big action” without **(1) context call** + **(2) proof window**.

## State Flags (shared language)
- `REGIME:` `STANDING` | `KNEELING`
- `MODE:` `UNDER` | `UP`
- `ENERGY:` `DRIVE` | `WITHDRAW` | `REDIRECT`
- `STATE:` `NORMAL` | `ALARM`
- `ARCHETYPE:` `MOBILITY` | `PRESSURE`
- `EXIT:` `FLEE` | `BACKSTEP` | `TURN-AWAY` | `PEEL/STRIP`

## Hotkeys (minimum viable OS set)
- [A-01 Context Laws (parent + laws)](#a-01)
- [A-04 Active-Link Identification](#a-04)
- [A-06 Hip-Line Alarm Gate](#a-06)
- [A-08 Passer Archetype (Mobility vs Pressure)](#a-08)
- [B-02 Handle Quality (2-of-3)](#b-02)
- [B-06 Re-Attachment Tempo](#b-06)
- [C-09 Recovery Sequencing](#c-09)
- [D-01 Repair-Step Window](#d-01)
- [D-16 Second Connection Rule](#d-16)
- [D-23 Anti-Exit Master](#d-23)

---

## Operator Loop (ASCII)

~~~
READ → DECIDE → CONNECT → FORCE REACTION → CONVERT → STABILIZE → ANTI-EXIT
 A     A/B      B         B/D             D         D           D

If behind / compressed:
A-06 (ALARM) → C-06 → C-09 → C-15 → back to READ/DECIDE

Quick Router (If X, run Y)
	•	If too many problems → A-04￼ → A-05￼
	•	If kneeling base feels stable → A-01a￼ → create proof → D-06￼
	•	If standing and they keep disengaging → A-02￼ (WITHDRAW) → D-04￼ → D-23￼
	•	If mobility circling → A-08￼ (MOBILITY) → B-09￼ → C-11￼ → C-10￼ → B-08￼ → D-01￼
	•	If pressure collapse → A-06￼ (ALARM) → C-06￼ → C-09￼ → C-15￼
	•	If you have grips but no progress → B-02￼ → B-03￼ → D-02￼
	•	If entries detach on first defense → B-16￼ → D-16￼
	•	If they backstep reset → D-22￼ → D-24￼ → D-23￼
	•	If they flee/reset range → D-22￼ → D-25￼ → D-23￼
	•	If they peel/strip → D-22￼ → D-26￼ → B-06￼ → D-16￼

Micro-Glossary (3 critical terms)
	•	PROOF: observable commitment (step/post/collapse/weight shift) that makes a conversion legal now.
	•	BEAT #1: the opponent’s first defensive action immediately after you connect (peel/step-away/turn-out).
	•	REPAIR-STEP WINDOW: the transition period while the opponent re-stabilizes base/posture after disruption; best conversion timing.
~~~
---

## Master Index

- [Bucket A — Decision Engines](#bucket-a--decision-engines)
  - [A-01 Context Laws Decision OS (Parent)](#a-01)
    - [A-01a Kneeling Shoulders–Hips Law OS](#a-01a)
    - [A-01b Standing Heels–Toes Law OS](#a-01b)
    - [A-01c Head Under / Head Over Mode Selection OS](#a-01c)
  - [A-02 Dynamic Energy Read OS](#a-02)
  - [A-03 Six-Element Passing Chain Model OS](#a-03)
  - [A-04 Active-Link Identification OS](#a-04)
  - [A-05 Early-Denial Triage OS](#a-05)
  - [A-06 Hip-Line Alarm Gate OS](#a-06)
  - [A-07 Retention State Machine OS](#a-07)
  - [A-08 Passer Archetype Identification OS](#a-08)
  - [A-09 Platform Validity Gate OS](#a-09)
  - [A-10 DLR Entry Validity Gate OS](#a-10)
  - [A-11 Clamp Validity Test OS (Closed Guard On/Off)](#a-11)

- [Bucket B — Control Engines](#bucket-b--control-engines)
  - [B-01 Connection-First OS](#b-01)
  - [B-02 Handle Quality System (2-of-3)](#b-02)
  - [B-03 Reaction-Driven Grip System](#b-03)
  - [B-04 Directional Job Assignment System](#b-04)
  - [B-05 Four-Limb Redundancy System](#b-05)
  - [B-06 Re-Attachment Tempo System](#b-06)
  - [B-07 Grip Loss Normalization System](#b-07)
  - [B-08 Steering-to-Step Map System](#b-08)
  - [B-09 First Contact Wins OS (Feet-on-Them)](#b-09)
  - [B-10 Asymmetry Creation OS](#b-10)
  - [B-11 Constant Threat Belief OS](#b-11)
  - [B-12 Leg Target Selection OS](#b-12)
  - [B-13 Threat Permanence Design OS](#b-13)
  - [B-14 Foot/Ankle Line Control OS](#b-14)
  - [B-15 Hips-Connected Attachment OS](#b-15)
  - [B-16 Sticky Connection Non-Negotiable OS](#b-16)

- [Bucket C — Recovery Engines](#bucket-c--recovery-engines)
  - [C-01 Knowledge/Denial Micro-Cycle OS](#c-01)
  - [C-02 Demarcation Theory OS](#c-02)
  - [C-03 Demarcation-to-Tool Router OS](#c-03)
  - [C-04 Essential Movement Selector OS](#c-04)
  - [C-05 Mobility-First Retention OS](#c-05)
  - [C-06 Defensive Framework Activation OS](#c-06)
  - [C-07 Frame Integrity OS](#c-07)
  - [C-08 Compression Management OS](#c-08)
  - [C-09 Recovery Sequencing OS](#c-09)
  - [C-10 Continuous Reinsertion OS](#c-10)
  - [C-11 Immediate Re-Square OS](#c-11)
  - [C-12 Mobility Defense Loop OS](#c-12)
  - [C-13 Pressure Defense Ladder OS](#c-13)
  - [C-14 Lock Formation Early-Denial OS](#c-14)
  - [C-15 Leg Reinsertion Terminal Step OS](#c-15)

- [Bucket D — Conversion Engines](#bucket-d--conversion-engines)
  - [D-01 Repair-Step Window OS](#d-01)
  - [D-02 Reaction Window Conversion System](#d-02)
  - [D-03 2-on-1 Ankle Primary Tool OS](#d-03)
  - [D-04 Distance Breaker OS](#d-04)
  - [D-05 Kneeling Entry Decision OS](#d-05)
  - [D-06 Proof-Gated Entry OS (Kneeling)](#d-06)
  - [D-07 Single-Leg Entry System OS](#d-07)
  - [D-08 Double-Leg Entry System OS](#d-08)
  - [D-09 Reverse Double-Leg Entry System OS](#d-09)
  - [D-10 Bridge-Platform Integration OS](#d-10)
  - [D-11 Momentum Entry OS](#d-11)
  - [D-12 X-Guard Triple-Attack Router OS](#d-12)
  - [D-13 RDLR as Anti-Pressure Bridge OS](#d-13)
  - [D-14 HQ Recognition OS](#d-14)
  - [D-15 DLR Outside-Control OS](#d-15)
  - [D-16 Second Connection Rule OS](#d-16)
  - [D-17 Entry-to-Consolidation Bridge OS](#d-17)
  - [D-18 Cross-Catch Consolidation OS](#d-18)
  - [D-19 Hip-Pin Consolidation OS](#d-19)
  - [D-20 Knee-Line Containment OS](#d-20)
  - [D-21 Platform-to-Hub Routing OS](#d-21)
  - [D-22 Exit-Based Hub Selection OS](#d-22)
  - [D-23 Anti-Exit Master OS](#d-23)
  - [D-24 Backstep Follow OS](#d-24)
  - [D-25 Flee Follow OS](#d-25)
  - [D-26 Peel/Strip Counter-Loop OS](#d-26)
  - [D-27 Stabilize-Then-Finish Governance OS](#d-27)

---

## Bucket A — Decision Engines

<a id="a-01"></a>
### A-01 — Context Laws Decision OS (Parent Router)

**Purpose (plain English)**  
Stop “random technique selection.” This router classifies the exchange so your actions match the opponent’s posture/base reality.

**Trigger**  
- Start of engagement  
- Any posture change (standing↔kneeling)  
- Before any committed entry / big movement  
- Any time options feel “too many”

**Inputs (what you read)**  
- `REGIME` (standing vs kneeling)  
- `MODE` availability (under vs up) based on head/hip relationship

**Outputs (what you decide)**  
- Regime call + mode call  
- Which downstream families are allowed (standing tools vs kneeling tools vs “come up first”)

**Run it (1-breath procedure)**  
1) `REGIME:` standing or kneeling?  
2) `MODE:` under available or must go up first?  
3) If unsure → default conservative: **create proof first** (don’t commit).

**DO / DON’T**  
- **DO:** Re-run immediately when they posture-change.  
- **DON’T:** Keep acting on a stale read (that’s how “nothing works”).

**Common mistakes it prevents**  
- Trying under-mode while opponent is hips-back/head-low.  
- Shooting into stable kneeling base with no proof.

**Linked sub-laws (the actual operators)**  
- [A-01a Kneeling Shoulders–Hips Law](#a-01a)  
- [A-01b Standing Heels–Toes Law](#a-01b)  
- [A-01c Head Under / Head Over Mode Selection](#a-01c)

---

<a id="a-01a"></a>
### A-01a — Kneeling Shoulders–Hips Law OS

**Purpose (plain English)**  
In kneeling exchanges, “is their upper body leading or is their base stacked?” determines whether entries are valid now or you must create proof first.

**Trigger**  
Opponent is kneeling or drops to knees.

**Reads (what matters)**  
- **Shoulders leading** (upper body pitched forward, posting likely)  
- **Hips stacked** (hips back under them, stable base, hard to off-balance)

**Decision logic (fast)**  
- Shoulders lead → expect **post/repair-step** → **convert on that window**  
- Hips stacked → **do not force entries** → **steer until proof appears**

**DO / DON’T**  
- **DO:** Treat a hand post as a permission slip (proof).  
- **DON’T:** Shoot under stacked hips and donate separation.

**Examples**  
- They kneel and lean forward to pressure: you steer → they post → you enter immediately.  
- They kneel upright and stable: you steer/base-shift first; entries come *after* a step/post.

**Failure signatures**  
- Stuffed entries with no forward progress.  
- You “touch legs” then lose them instantly (no base compromise).

**Metrics**  
- % kneeling entries initiated **on proof** (post/step/collapse)  
- Proof→entry initiation time (should be immediate)

**Links**  
- Next: [A-02 Energy Read](#a-02), [D-05 Kneeling Entry Decision](#d-05), [D-06 Proof-Gated Entry](#d-06)

---

<a id="a-01b"></a>
### A-01b — Standing Heels–Toes Law OS

**Purpose (plain English)**  
Standing weight distribution predicts whether the opponent will drive, stabilize, or retreat—so you stop attacking into stability and start attacking during motion.

**Trigger**  
Opponent is standing.

**Reads**  
- **Toes-loaded** (forward committed, driving pressure, corrective steps likely)  
- **Heels-loaded** (anchored / ready to withdraw, step-away likely)

**Decision logic (fast)**  
- Toes-loaded → **expect correction step** → intercept/convert on motion  
- Heels-loaded → **force step map** → don’t chase; create predictable stepping

**DO / DON’T**  
- **DO:** Attack on the step, not after the step.  
- **DON’T:** Chase ankles against a retreat-ready stance without forcing commitment.

**Examples**  
- Forward committed: you steer → they must step → you intercept the step.  
- Retreat-ready: you constrain options (step map) → their retreat becomes predictable → you attach.

**Failure signatures**  
- Touch-and-lose leg contacts.  
- Repeated long-range resets because you attacked after they stabilized.

**Metrics**  
- % entries initiated during opponent motion (vs static)  
- Reset events after “attempted engagement”

**Links**  
- Next: [B-08 Step Map](#b-08), [D-03 2-on-1 Ankle Tool](#d-03), [D-04 Distance Breaker](#d-04)

---

<a id="a-01c"></a>
### A-01c — Head Under / Head Over Mode Selection OS

**Purpose (plain English)**  
Select `MODE` correctly: under-mode is not always available. If head is low and hips are back, you often must “come up” first.

**Trigger**  
Always active; re-check anytime posture changes.

**Reads**  
- Head height vs opponent hip withdrawal  
- “Can I actually get underneath without being separated?”

**Decision logic (fast)**  
- Head high / access under them exists → `MODE: UNDER`  
- Head low + opponent hips back / posture denying under → `MODE: UP` first

**DO / DON’T**  
- **DO:** Switch modes without attachment to your preferred plan.  
- **DON’T:** Repeat under-attempts into hips-back posture.

**Examples**  
- They posture/hips back: you come up, reattach, force a step, then under becomes available later.  
- They’re tall and committed: under-mode is live immediately.

**Failure signatures**  
- Chronic separation right as you try to go under.  
- “Almost” entries that never connect because posture denies them.

**Metrics**  
- Under-attempts that end in separation (%)  
- Mode switch speed (how quickly you stop forcing the wrong mode)

**Links**  
- Next: [A-02 Energy Read](#a-02), [D-11 Momentum Entry](#d-11), [C-11 Re-Square](#c-11)

<a id="a-02"></a>
### A-02 — Dynamic Energy Read OS (`DRIVE` / `WITHDRAW` / `REDIRECT`)

**Purpose (plain English)**  
Predict the opponent’s *next corrective action* so you act during transition windows instead of attacking into stability.

**Trigger**  
- Any shift in pressure direction  
- Any stepping/circling/backing-out behavior  
- Immediately after you disrupt/deny something (they must “fix”)

**Reads (what matters)**  
- `DRIVE:` pressure/weight moving **into you** (commitment forward)  
- `WITHDRAW:` pressure/weight moving **away** (reset attempt)  
- `REDIRECT:` pressure moving **around** you (angle hunting)

**Decision logic (fast)**

DRIVE    → expect post/repair-step windows → convert on that beat
WITHDRAW → expect disengage/reset         → intercept + reattach immediately
REDIRECT → expect angle accumulation      → re-square NOW, not later

**Run it (2-step procedure)**  
1) Name the energy: DRIVE / WITHDRAW / REDIRECT.  
2) Pair it with the correct priority:
   - DRIVE → force/harvest proof windows ([D-01](#d-01), [D-02](#d-02))
   - WITHDRAW → deny reset with sticky connection ([D-23](#d-23))
   - REDIRECT → deny angle with re-square + reinsertion ([C-11](#c-11), [C-10](#c-10))

**DO / DON’T**  
- **DO:** Update instantly when the energy changes (no plan loyalty).  
- **DON’T:** Chase after a WITHDRAW; you arrive late and they’re stable.

**Examples (common)**  
- You steer and they *step hard to stabilize* → DRIVE window → enter now.  
- You threaten and they *back out to reset* → WITHDRAW → follow, keep one connection.  
- They circle to your flank → REDIRECT → re-square before they connect angle to level.

**Failure signatures**  
- You “do the right move” but at the wrong time (stability vs transition).  
- You keep losing angle while hand-fighting.  
- You allow repeated clean resets.

**Metrics**  
- % conversions initiated during transitions (step/post/repair-step)  
- Reset attempts denied after WITHDRAW reads  
- Angle-loss events after REDIRECT reads

**Links**  
- Upstream: [A-01 Context Laws](#a-01)  
- Downstream: [A-04 Active Link](#a-04), [C-11 Re-Square](#c-11), [D-01 Repair-Step](#d-01), [D-23 Anti-Exit](#d-23)

---

<a id="a-03"></a>
### A-03 — Six-Element Passing Chain Model OS

**Purpose (plain English)**  
Stop thinking in “pass names.” Diagnose the *requirement chain* the passer must build and break it early.

**The chain (order matters)**  
1) **Distance** (closing space / denying you space)  
2) **Grip** (meaningful attachments that survive movement)  
3) **Angle** (getting to your hip line / flank)  
4) **Level** (getting chest/hips into winning height relationship)  
5) **Penetration** (entering past your frames/legs)  
6) **Pin** (stabilizing control so you cannot recover)

**Trigger**  
- Any time passing is progressing  
- Any time you feel overwhelmed and need a clean diagnosis

**Read (what matters)**  
Identify the **earliest dominant link** that explains the current threat.

**Run it (fast)**  
1) Ask: “Which link are they building right now?”  
2) Deny that link (or an earlier one if possible).  
3) Reassess immediately (chain shifts after denial).

**DO / DON’T**  
- **DO:** Spend most of your defense at Distance/Grip/Angle (cheap).  
- **DON’T:** Live in Penetration/Pin defense (expensive lifestyle).

**Examples**  
- They haven’t connected grips yet → distance management is the real fight, not late framing.  
- They have grips but no angle yet → break grips / re-square before they flank.  
- Angle is being won → re-square first, even if grips remain.

**Failure signatures**  
- You win grip exchanges but still get passed (angle was the real link).  
- You constantly “survive” late but never reset upstream.

**Metrics**  
- Early vs late denial ratio (Distance/Grip/Angle vs Penetration/Pin)  
- Time spent in emergency states (Penetration/Pin)  
- Correct link identification rate (self-audit after round)

**Links**  
- Downstream: [A-04 Active Link](#a-04), [A-05 Triage](#a-05), [C-01 Micro-Cycle](#c-01)

---

<a id="a-04"></a>
### A-04 — Active-Link Identification OS (Single Problem Selection)

**Purpose (plain English)**  
When multiple things feel threatening, select the *one* link to solve first so you stop defending symptoms.

**Trigger**  
- “Too many problems” feeling  
- Pressure spike  
- Immediately after any denial or scramble (the active link changes)

**Inputs**  
- Current chain state (from [A-03](#a-03)) + `STATE` (NORMAL/ALARM from [A-06](#a-06))

**Outputs**  
- One declared “active link” (the first thing you deny)

**Run it (fast)**  
1) Name the earliest dominant link: Distance / Grip / Angle / Level / Penetration / Pin.  
2) Deny it.  
3) Re-run immediately (do not assume the problem stayed the same).

**DO / DON’T**  
- **DO:** Solve one link fully, then reassess.  
- **DON’T:** Split attention across grip + angle + level simultaneously (you’ll lose all three).

**Examples**  
- They are circling (angle threat) and also have a sleeve/hand tie: active link is **Angle** (if you lose flank, grips get worse).  
- They are compressing without angle yet: active link is **Distance/Level** (stop collapse before it becomes penetration).

**Failure signatures**  
- You “fix grips” while they run around.  
- You frame late while penetration is already occurring.

**Metrics**  
- Correct first-link calls (review after round)  
- Denials that prevent next-link progression (%)  
- Reassessment frequency (should be high; the link changes often)

**Links**  
- Upstream: [A-03 Chain Model](#a-03)  
- Downstream: [A-05 Triage](#a-05), [C-01 Micro-Cycle](#c-01), [A-06 Hip-Line Gate](#a-06)

---

<a id="a-05"></a>
### A-05 — Early-Denial Triage OS (Priority Order)

**Purpose (plain English)**  
When you’re behind or confused, apply a fixed priority order so you stop bleeding into emergencies.

**Trigger**  
- You feel behind in the exchange  
- Passing is accelerating  
- You can’t decide what to defend first

**Inputs**  
- Active link guess + pin imminence assessment

**Outputs**  
- A prioritized denial plan (what to address first)

**Default priority (earlier = cheaper)**  
1) Distance  
2) Grip  
3) Angle  
4) Level  
5) Penetration (emergency)  
6) Pin (emergency)

**Run it (fast)**  
1) If pin is imminent → survive first (frames/wedges), then immediately return to upstream links.  
2) If pin not imminent → solve earliest live link from the list.

**DO / DON’T**  
- **DO:** After any emergency survival, immediately re-run [A-04](#a-04) to fix upstream cause.  
- **DON’T:** “Survive then chill.” Survival without upstream repair repeats the emergency.

**Examples**  
- You’re getting smashed but not pinned yet: active priority is **Distance/Level**—stop collapse early.  
- You are pinned: do [A-06](#a-06) (ALARM) → [C-06](#c-06) framework → [C-15](#c-15) reinsertion → back to early links.

**Failure signatures**  
- Permanent late defense (always penetration/pin).  
- You escape but get re-collapsed immediately.

**Metrics**  
- Early:late denial ratio  
- Pin events per round  
- Time from emergency → return to early denial

**Links**  
- Upstream: [A-04 Active Link](#a-04)  
- Downstream: [A-06 Hip-Line Alarm](#a-06), [C-13 Pressure Ladder](#c-13), [C-09 Sequencing](#c-09)

Say “next” and I’ll continue with A-06 and A-07 (expanded, including crisp alarm criteria and state transitions), then A-08.

<a id="a-06"></a>
### A-06 — Hip-Line Alarm Gate OS (`STATE: NORMAL` vs `STATE: ALARM`)

**Purpose (plain English)**  
A binary gate that prevents the most common retention error: using “mobility solutions” when you are already close to being pinned. It declares which priority stack is legal right now.

**Trigger**  
- Any sudden pressure spike  
- Knee line collapses / hips threatened  
- You feel “one beat from getting flattened”  
- Any time you’re unsure whether to move or frame

**Reads (alarm criteria — keep it simple)**
Alarm is **ON** if **any** of these are true:
- Opponent’s chest/hip line is **past your primary leg barrier** (they’re “in”)  
- Your **knee line is cleared or stapled** and you cannot reinsert immediately  
- Opponent can **settle weight** without you being able to re-square  
- Your frames are being collapsed and **you’re being turned** (pin mechanics forming)

Alarm is **OFF** if:
- You still have **functional barriers** (legs between you and them) *or*  
- You can re-square and reinsert legs **without** needing a survival frame first

**Outputs**  
- `STATE: ALARM` → structure-first legality (frames/wedges, space budgeting)  
- `STATE: NORMAL` → mobility-first legality (re-square, reinsertion, step-map denial)

**Run it (fast)**  
1) Ask: “Am I about to be pinned if I try to move freely?”  
2) If yes → `ALARM ON` (structure-first).  
3) If no → `ALARM OFF` (mobility-first).

**DO / DON’T**  
- **DO:** Switch states instantly when the gate flips.  
- **DON’T:** Stay in NORMAL while pin mechanics are forming (guaranteed collapse).  
- **DON’T:** Stay in ALARM after you’ve regained space (you’ll stall and get run around).

**Examples**  
- Legs cleared + chest heavy + you can’t re-square → ALARM (frames first).  
- They’re circling but you still have feet on them and can re-square → NORMAL (mobility first).

**Failure signatures**  
- You “pummel legs” while getting flattened.  
- You “frame forever” against a mobility passer and lose angle.

**Metrics**  
- Alarm recognition latency (beats from danger cue → correct state)  
- % ALARM events resolved without pin  
- Pins occurring after missed ALARM calls (should trend to zero)

**Links**  
- Upstream: [A-04 Active Link](#a-04), [A-05 Triage](#a-05)  
- Downstream (ALARM): [C-06 Framework Activation](#c-06), [C-07 Frame Integrity](#c-07), [C-08 Compression Mgmt](#c-08), [C-15 Reinsertion Terminal](#c-15)  
- Downstream (NORMAL): [C-11 Re-Square](#c-11), [C-10 Continuous Reinsertion](#c-10), [C-12 Mobility Loop](#c-12)

---

<a id="a-07"></a>
### A-07 — Retention State Machine OS (`STATE: NORMAL` ↔ `STATE: ALARM`)

**Purpose (plain English)**  
Give you two clean playbooks. NORMAL is “re-square and rebuild barriers.” ALARM is “survive compression, create space, then rebuild barriers.” No mixed priorities.

**Trigger**  
- Immediately after running [A-06](#a-06)  
- Any time the exchange changes (space gained/lost, angle changes, pressure changes)

**Inputs**  
- `STATE` from A-06  
- Space availability (do you have usable space or are you compressed?)

**Outputs**  
- A legal priority stack for the next 2–5 seconds  
- A state transition rule (when to switch)

#### NORMAL Playbook (alarm OFF)
**Goal:** keep opponent in front, restore barriers, restore connection.
1) **Re-square** hips/shoulders ([C-11](#c-11))  
2) **Reinsert legs**/lanes ([C-10](#c-10))  
3) **Reattach** handles + redundancy ([B-06](#b-06), [B-05](#b-05))  
4) **Convert** on their repair-step ([D-01](#d-01))

**DO:** move first, then frame only if needed.  
**DON’T:** freeze in frames while they circle.

#### ALARM Playbook (alarm ON)
**Goal:** stop pin completion, create space, then rebuild guard.
1) **Framework** (wedges/frames) ([C-06](#c-06), [C-07](#c-07))  
2) **Budget space** (don’t waste openings) ([C-08](#c-08))  
3) **Sequence recovery** Space→Align→Reinsert→Attach ([C-09](#c-09))  
4) **Terminal step:** legs back in front ([C-15](#c-15))

**DO:** let frames buy time; spend that time reinserting legs.  
**DON’T:** push (fatigue), or try “mobility escapes” without structure.

**State transition rules**
- Switch **NORMAL → ALARM** the moment hip-line risk appears (A-06 flips ON).  
- Switch **ALARM → NORMAL** as soon as you have usable space + legs can reinsert (don’t remain frame-locked).

**Failure signatures**  
- “Half mobility, half frames” (the classic incoherent defense).  
- Staying in ALARM after you’ve already escaped compression (stalls you).

**Metrics**  
- Time spent in ALARM state (should shrink with skill)  
- % transitions where you switch within 1 beat of gate change  
- % defenses ending with legs-in + at least one handle (C-15 + B-06)

**Links**  
- Upstream: [A-06 Hip-Line Alarm Gate](#a-06)  
- Downstream: [C-09 Sequencing](#c-09), [C-12 Mobility Loop](#c-12), [C-13 Pressure Ladder](#c-13)

---

<a id="a-08"></a>
### A-08 — Passer Archetype Identification OS (`ARCHETYPE: MOBILITY` vs `ARCHETYPE: PRESSURE`)

**Purpose (plain English)**  
Select the correct defense module. Mobility passers win with angle and circling; pressure passers win with collapse, locks, and stabilization. Wrong archetype = wrong tools.

**Trigger**  
- First 1–2 beats of any pass attempt  
- Any time the opponent changes behavior mid-exchange

**Reads (simple cues)**
- `MOBILITY:` circling, lateral steps, “run around,” light contact, fast angle hunting  
- `PRESSURE:` closing hips/chest, clamping/locking, slowing you, stacking/compressing, stabilizing before progressing

**Outputs**  
- `ARCHETYPE` call + the correct module priority

**Run it (fast)**
1) Classify: Are they trying to **get around** (mobility) or **go through/into** (pressure)?  
2) Deploy the matching module:
   - MOBILITY → **front-facing** KPI (feet connection + re-square loop)  
   - PRESSURE → **deny lock early**; if late, **structure-first ladder**

**DO / DON’T**  
- **DO:** Re-run archetype after any “style switch” (many passers alternate).  
- **DON’T:** Use pressure defenses vs mobility (you’ll get run around).  
- **DON’T:** Use mobility defenses under compression (you’ll get pinned).

**Examples**
- They circle hard and guide your legs aside → MOBILITY → [B-09](#b-09) + [C-11](#c-11) loop.  
- They settle chest-to-hip, connect hands, and clamp → PRESSURE → [C-14](#c-14) early denial or [C-13](#c-13) ladder.

**Failure signatures**
- You “frame early” and they simply step around (misread mobility).  
- You “try to re-square” while being smashed flat (misread pressure).

**Metrics**
- Correct archetype calls (self-review)  
- Angle-loss events while in MOBILITY module  
- Pin events while in PRESSURE module

**Links**
- Downstream (MOBILITY): [B-09 Feet-on-Them](#b-09), [B-10 Asymmetry](#b-10), [C-11 Re-Square](#c-11), [C-12 Mobility Loop](#c-12)  
- Downstream (PRESSURE): [C-14 Lock Early-Denial](#c-14), [C-13 Pressure Ladder](#c-13), [A-06 Alarm Gate](#a-06)

<a id="a-09"></a>
### A-09 — Platform Validity Gate OS (X / RDLR / HQ)

**Purpose (plain English)**  
Prevent “platform hope.” A platform is only valid if it **restricts** and **survives the first defensive beat**. If it doesn’t, you’re just sitting in contact until they peel and reset.

**Trigger**  
- You are about to enter a platform (X / RDLR / HQ)  
- You “land” in a platform from a scramble  
- You feel unsure if you should commit deeper or back out

**Reads (validity tests)**
A platform is **VALID** only if all are true:
1) **Proof exists:** opponent is in a transition (step/post/turn/repair-step) or weight is committed.  
2) **Sticky connection:** you can keep *at least one* meaningful connection through their first peel/step-away attempt.  
3) **Restriction present:** their easiest reset route (step away / peel / backstep) is not immediately free.

Platform is **INVALID** if any are false:
- no proof (stable base),
- first peel clears everything,
- they can step away and you can’t follow with attachment.

**Outputs**  
- VALID → permission to commit to platform + install redundancy + route to hub  
- INVALID → return to connection/steering and create proof first (don’t sink time)

**Run it (fast)**
1) “Do I have proof (transition/commitment)?”  
2) “Will I keep one connection through defense beat #1?”  
3) “Does this platform restrict an exit right now?”  
If any “no” → platform is invalid.

**DO / DON’T**  
- **DO:** Treat the first defensive beat as the exam—pass it or abort.  
- **DON’T:** Stall inside invalid platform contact.

**Examples**
- You enter as they step/turn and you maintain a hook/connection through the peel → VALID.  
- You enter on stable base and they peel once and step away → INVALID.

**Failure signatures**  
- “I get to X/RDLR but it never works.” (Usually failing the validity gate.)  
- Immediate peel → full reset; repeated.

**Metrics**  
- Platform false-start rate (invalid entries per round)  
- First-peel survival rate  
- Platform→consolidation or platform→hub conversion rate

**Links**  
- Upstream: [A-01 Context Laws](#a-01), [A-02 Energy Read](#a-02), [B-16 Sticky Connection](#b-16)  
- Downstream: [D-10 Bridge-Platform Integration](#d-10), [D-16 Second Connection](#d-16), [D-21 Platform-to-Hub Routing](#d-21), [D-23 Anti-Exit](#d-23)

---

<a id="a-10"></a>
### A-10 — DLR Entry Validity Gate OS (Proof Before Hook)

**Purpose (plain English)**  
DLR is not “a hook.” It is a control promise. This gate prevents you from throwing a hope-hook that gets peeled instantly and resets the exchange.

**Trigger**  
- You are about to establish DLR from open distance  
- You are re-engaging after a reset  
- You have “hook access” but are unsure if it will hold

**Reads (validity tests)**
DLR entry is **ALLOWED** only if:
1) **Proof exists:** opponent is stepping/turning/committed (not stable and ready to disengage).  
2) **Outside control will exist:** you can create an outside track that blocks easy step-away.  
3) **Beat #1 survival:** you can keep at least one connection through their first peel/step-away attempt.

DLR entry is **DENIED** if:
- they can step away cleanly,
- first peel removes everything,
- you cannot immediately add a second connection.

**Outputs**  
- ALLOWED → enter DLR + install redundancy + force step map  
- DENIED → create proof first (steer to a step/commitment), then re-attempt

**Run it (fast)**
1) “Are they stable or transitioning?” (Need transitioning.)  
2) “Can I prevent a clean step-away?”  
3) “Can I survive peel #1?”  
If any “no” → don’t hook.

**DO / DON’T**  
- **DO:** Enter DLR on motion (step/turn) and immediately add second connection.  
- **DON’T:** Use DLR as a “pause position” after a reset.

**Examples**
- They step forward to re-engage and you hook on the step + maintain outside control → ALLOWED.  
- They’re upright, hips back, ready to disengage, and you hook from far → DENIED.

**Failure signatures**  
- DLR “turns off” instantly.  
- You hook, they peel, and you’re back at zero repeatedly.

**Metrics**  
- DLR false-start rate  
- Peel #1 survival rate  
- Forced steps/posts per minute from DLR (if near zero, DLR isn’t functioning)

**Links**  
- Upstream: [A-01b Standing Heels–Toes](#a-01b), [B-16 Sticky Connection](#b-16)  
- Downstream: [D-15 DLR Outside-Control](#d-15), [D-16 Second Connection](#d-16), [B-08 Step Map](#b-08), [D-23 Anti-Exit](#d-23)

---

<a id="a-11"></a>
### A-11 — Clamp Validity Test OS (Closed Guard On/Off)

**Purpose (plain English)**  
Closed guard is only valuable if it **clamps**: it must restrict posture, distance, and stand-up. Loose closed guard is a time sink that gives clean resets.

**Trigger**  
- You close guard  
- You’re deciding whether to close guard vs stay open  
- Opponent starts posturing/standing inside your closed guard

**Reads (validity tests)**
Clamp is **ON (valid)** only if at least two are true:
1) **Posture restriction:** they cannot posture up freely.  
2) **Stand-up restriction:** they cannot stand without immediate cost.  
3) **Distance restriction:** they cannot open and back out cleanly.

Clamp is **OFF (invalid)** if:
- they posture at will,
- they stand with no consequence,
- they open and disengage cleanly.

**Outputs**  
- Clamp ON → permission to run closed-guard offense/governance  
- Clamp OFF → immediate correction: rebuild clamp mechanics or exit back to open systems

**Run it (fast)**
1) “Can they posture up freely?”  
2) “Can they stand freely?”  
3) “Can they open and disengage freely?”  
If two or more answers are “yes” → clamp is OFF.

**DO / DON’T**  
- **DO:** Treat clamp OFF as a trigger to transition—don’t “hang on.”  
- **DON’T:** Assume closed guard is automatically control.

**Examples**
- They stand and your guard opens with no penalty → clamp was OFF; you should have transitioned earlier.  
- They cannot posture without being pulled back down and cannot stand cleanly → clamp ON.

**Failure signatures**  
- Closed guard becomes a “rest” that opponent uses to stand/open/reset.  
- You attack while posture is free and get immediately neutralized.

**Metrics**  
- Clean stand-ups allowed from your closed guard  
- Clamp validity rate (how often closed guard actually restricts)  
- Time clamp OFF → you transition (should be quick)

**Links**  
- Upstream: [A-01 Context Laws](#a-01)  
- Downstream: [D-27 Stabilize-Then-Finish Governance](#d-27), [D-23 Anti-Exit](#d-23), [B-06 Re-Attach Tempo](#b-06)

## Bucket B — Control Engines

<a id="b-01"></a>
### B-01 — Connection-First OS

**Purpose (plain English)**  
You don’t control what you’re not attached to. This OS makes “attachment before movement” your default so the opponent can’t reset distance for free.

**Trigger**  
- Start of engagement  
- Any time contact breaks  
- Any time you’re about to initiate a big movement/entry  
- After any strip/peel event

**Reads (what matters)**  
- Do you have **a handle** that (a) survives a step and (b) allows steering?

**Outputs**  
- A **durable connection** that survives at least one opponent step  
- Permission to run steering, proof creation, and conversion

**Run it (fast)**  
1) Attach to something meaningful (not fingertips, not cosmetic touch).  
2) Test immediately: “If they step once, do I still have control?”  
3) If no → replace (do not move big without a handle).

**DO / DON’T**  
- **DO:** Treat connection as the steering wheel, not a bonus.  
- **DON’T:** Move first and hope to grab later (that creates resets).

**Examples**  
- You reach for an entry from distance with no durable attachment → they step away → you’re chasing. Connection-first prevents that.  
- You get stripped → instead of pausing, you immediately rebuild one handle, then two.

**Failure signatures**  
- “I keep ending up at long range.” (Movement without connection.)  
- You enter but get peeled instantly (connection wasn’t durable).

**Metrics**  
- Time-to-first durable connection from reset  
- % exchanges where connection survives the first opponent step

**Links**  
- Upstream: [A-01 Context Laws](#a-01), [A-02 Energy Read](#a-02)  
- Downstream: [B-02 Handle Quality](#b-02), [B-05 Redundancy](#b-05), [B-06 Re-Attach Tempo](#b-06)

---

<a id="b-02"></a>
### B-02 — Handle Quality System (2-of-3 Rubric)

**Purpose (plain English)**  
Stop “collecting grips.” Decide if a handle is worth building around in 1–2 beats.

**Trigger**  
- The moment you establish any grip/attachment  
- Any time you feel you’re holding but nothing is changing

**Reads (the rubric — score 0/1 each)**  
1) **Survivability:** survives one opponent step/peel attempt  
2) **Reactivity:** forces a reaction (step/post/posture change) within 1–2 beats  
3) **Continuity:** directly connects to your next action (proof/entry/upgrade/reattach)

**Outputs**  
- **KEEP + BUILD** (≥2/3) or **REPLACE/UPGRADE** (≤1/3)

**Run it (fast)**  
1) Score the handle instantly.  
2) If ≥2/3 → treat as primary; install second connection.  
3) If ≤1/3 → treat as temporary; replace immediately.

**DO / DON’T**  
- **DO:** Replace weak handles fast; tempo beats strength.  
- **DON’T:** Fight to keep a 1/3 handle; it’s a time sink.

**Examples**  
- A grip feels strong but doesn’t change their posture and breaks on a step → 1/3 → replace.  
- A leg line control that survives a step and immediately forces a post → 2/3+ → build around it.

**Failure signatures**  
- Static tug-of-war with no steps/posts.  
- You keep “strong” grips that don’t create proof windows.

**Metrics**  
- % handles scoring ≥2/3  
- Replacement latency for failed handles (beats)

**Links**  
- Upstream: [B-01 Connection-First](#b-01)  
- Downstream: [B-04 Directional Job](#b-04), [B-03 Reaction-Driven Grip](#b-03), [B-05 Redundancy](#b-05)

---

<a id="b-03"></a>
### B-03 — Reaction-Driven Grip System (Force Step / Post / Posture)

**Purpose (plain English)**  
Control is measured by *reactions you force*, not grips you hold. This OS turns handles into proof windows.

**Trigger**  
- Immediately after any handle becomes “keepable” (B-02 ≥2/3)  
- Any time opponent is stable and you need to create proof

**Reads (what matters)**  
- What reaction is most available right now:
  - **Step** (base correction)
  - **Post** (hands-down)
  - **Posture change** (head/shoulder line displaced)

**Outputs**  
- A forced reaction within 1–2 beats  
- A short conversion window (repair-step window)

**Run it (fast)**  
1) Pick the reaction you are forcing (step / post / posture).  
2) Apply directional pressure until it happens (1–2 beats).  
3) Convert immediately during the reaction window ([D-02](#d-02), [D-01](#d-01)).

**DO / DON’T**  
- **DO:** Convert during their reaction, not after it.  
- **DON’T:** Accept “stable opponent + I have grips” as progress.

**Examples**  
- You pull posture → they post → that post is your permission slip to enter/upgrade.  
- You steer base → they step to repair → you attack during the step, not after they plant.

**Failure signatures**  
- You force reactions but gain nothing (conversion latency).  
- You hold grips and opponent remains stable and confident.

**Metrics**  
- Reaction rate within 1–2 beats  
- Reaction→conversion time (beats)  
- % reactions that produce tangible progress (entry/control)

**Links**  
- Upstream: [B-02 Handle Quality](#b-02), [A-02 Energy Read](#a-02)  
- Downstream: [D-01 Repair-Step Window](#d-01), [D-02 Reaction Window Conversion](#d-02), [B-08 Step Map](#b-08)

---

<a id="b-04"></a>
### B-04 — Directional Job Assignment System (Every Handle Has One Job)

**Purpose (plain English)**  
A handle without a job is just a hold. This OS forces you to assign a single directional task to every attachment so steering becomes automatic.

**Trigger**  
- The moment you take a grip/attach to a leg/hip/arm  
- Any time you feel “I’m connected but not sure what to do”

**Reads (what matters)**  
- Which direction will most reliably force a step/post/posture shift *right now* given their stance and `ENERGY`?

**Outputs**  
- One declared job + the reaction you are hunting

**Job menu (choose ONE primary)**  
- **Break posture** (pull head/shoulders out of line)  
- **Turn shoulders** (create rotation)  
- **Force step** (make base move)  
- **Force post** (hands-down)  
- **Block retreat** (deny WITHDRAW reset)

**Run it (fast)**  
1) Name the job in one sentence (“This handle is to force a step.”).  
2) Execute until reaction occurs or the handle fails the 2-of-3 test.  
3) If reaction doesn’t appear quickly, upgrade/replace the handle.

**DO / DON’T**  
- **DO:** Keep the job measurable (step/post/posture shift).  
- **DON’T:** Say “control” without direction (that’s how you stall).

**Examples**  
- Opponent is WITHDRAW-ing: job becomes “block retreat + reattach,” not “pull harder.”  
- Opponent is DRIVE-ing: job becomes “force post/step” then convert on repair-step.

**Failure signatures**  
- You accumulate grips but nothing changes.  
- You switch directions randomly with no forced reactions.

**Metrics**  
- % handles with explicitly stated job  
- Job success rate (reaction achieved within 1–2 beats)

**Links**  
- Upstream: [B-02 Handle Quality](#b-02), [A-02 Energy Read](#a-02)  
- Downstream: [B-03 Reaction-Driven Grip](#b-03), [B-08 Step Map](#b-08), [D-01 Repair-Step](#d-01)

<a id="b-05"></a>
### B-05 — Four-Limb Redundancy System (Two Points Minimum)

**Purpose (plain English)**  
Single-point control collapses on one peel. Redundancy makes control survive stripping long enough to convert.

**Trigger**  
- Immediately after establishing any primary handle  
- Any time you notice you’re “one peel away from nothing”

**Reads**  
- Connection count: 1 point vs 2+ points  
- Opponent’s peel/strip readiness (hands active, step-away pattern)

**Outputs**  
- ≥2 connection points that remain functional if one is stripped

**Run it (fast)**  
1) Establish first handle.  
2) Install second connection within 1–2 beats.  
3) Only then commit to deeper actions.

**DO / DON’T**  
- **DO:** Treat “two points” as the price of stability.  
- **DON’T:** Start finishing/entering from single-point contact.

**Failure signatures**  
- First peel clears everything.  
- You keep “almost had it” grips that never stabilize.

**Metrics**  
- Time to second connection after first contact  
- First-peel survival rate

**Links**  
- Upstream: [B-02](#b-02), [B-01](#b-01)  
- Downstream: [D-16](#d-16), [B-06](#b-06)

---

<a id="b-06"></a>
### B-06 — Re-Attachment Tempo System (Replace in 1 Beat)

**Purpose (plain English)**  
Grip loss is normal. The failure is the pause after loss. This OS enforces immediate replacement.

**Trigger**  
- Any strip/peel/break in contact  
- Any time you feel a “dead beat” after losing a handle

**Reads**  
- What got stripped + what remains connected (if anything)

**Outputs**  
- Immediate replacement handle + rebuild to redundancy

**Run it (fast)**  
1) Strip happens → replace within 1 beat.  
2) Rebuild second connection (B-05).  
3) Resume forcing reactions (B-03).

**DO / DON’T**  
- **DO:** Replace first, think second.  
- **DON’T:** Chase without attachment.

**Failure signatures**  
- Reset to long range after every peel.  
- You arrive late after WITHDRAW.

**Metrics**  
- Strip → replacement time  
- Dead-beat count per round

**Links**  
- Upstream: [B-05](#b-05)  
- Downstream: [D-23](#d-23), [B-07](#b-07)

---

<a id="b-07"></a>
### B-07 — Grip Loss Normalization OS (No Emotional Reset)

**Purpose (plain English)**  
Prevents mental reset. Grip loss becomes a predictable beat in your loop: lose → replace → rebuild → steer.

**Trigger**  
- Any time you lose a grip and feel “reset mode”

**Reads**  
- Whether you still have one connection (yes/no)

**Outputs**  
- Immediate continuation of the control loop

**Run it (fast)**  
1) Label strip as normal.  
2) Replace (B-06).  
3) Add second connection (B-05).  
4) Force reaction again (B-03).

**DO / DON’T**  
- **DO:** Run the loop automatically.  
- **DON’T:** Stop and re-plan after every peel.

**Failure signatures**  
- Tempo collapse after first strip.  
- You lose initiative and become reactive.

**Metrics**  
- Dead-beat count after strips  
- Replacement consistency under fatigue

**Links**  
- Reinforces: [B-06](#b-06) and [B-05](#b-05)

---

<a id="b-08"></a>
### B-08 — Steering-to-Step Map System (Constrain Foot Options)

**Purpose (plain English)**  
If they can step anywhere, you don’t control base. This system narrows their step options so reactions become predictable and exploitable.

**Trigger**  
- You have a durable handle but opponent remains mobile  
- Opponent is circling/stepping to reset

**Reads**  
- Which steps are currently available to them (free vs constrained)  
- Whether your handle direction actually moves their base

**Outputs**  
- A constrained “step map” that yields forced steps/posts (proof windows)

**Run it (fast)**  
1) Use directional handles to force weight commitment.  
2) Observe their forced step direction.  
3) Convert on the step (repair-step window).

**DO / DON’T**  
- **DO:** Create predictability; then intercept.  
- **DON’T:** Chase free footwork.

**Failure signatures**  
- Endless circling; you burn energy.  
- You never get proof (no forced steps/posts).

**Metrics**  
- Forced steps/posts per minute  
- Conversion rate on forced step windows

**Links**  
- Upstream: [B-03](#b-03), [B-04](#b-04)  
- Downstream: [D-01](#d-01), [D-11](#d-11), [C-11](#c-11)

<a id="b-09"></a>
### B-09 — First Contact Wins OS (Feet-on-Them Interface)

**Purpose (plain English)**  
Against mobile passing, feet contact is your steering interface. If feet aren’t meaningfully connected, the passer guides your legs aside and wins angle for free.

**Trigger**  
- `ARCHETYPE: MOBILITY` (circling/run-around)  
- Any time your legs are being pushed/stapled aside without resistance

**Reads**  
- Feet connection status: ON (meaningful contact) vs OFF (floating)  
- Angle drift starting (opponent moving off-center)

**Outputs**  
- Active feet-on-them contact that blocks free steering and supports re-square

**Run it (fast)**  
1) Establish meaningful foot contact early.  
2) Keep it through their first circle attempt.  
3) Use it to re-square and reinsert lanes.

**DO / DON’T**  
- **DO:** Treat feet contact as non-negotiable vs mobility.  
- **DON’T:** Hand-fight while your feet are disconnected.

**Failure signatures**  
- “They just push my legs aside and go.”  
- You chase with hands; hips lag; angle accumulates.

**Metrics**  
- Time from reset → feet contact ON  
- “Free leg push” events allowed per round

**Links**  
- Upstream: [A-08](#a-08)  
- Downstream: [C-11](#c-11), [C-12](#c-12), [B-10](#b-10)

---

<a id="b-10"></a>
### B-10 — Asymmetry Creation OS (Don’t Let Both Legs Be Solved)

**Purpose (plain English)**  
Symmetrical legs are easy to staple/clear together. Asymmetry forces the passer to solve one side at a time, slowing the pass chain.

**Trigger**  
- Opponent starts stapling/scooping/steering both legs together  
- You notice both legs drifting into the same height/line

**Reads**  
- Symmetry: both legs same line/height and easily bundled  
- Lane status: do you still have at least one active lane?

**Outputs**  
- Staggered leg structure that preserves at least one active lane + supports re-square

**Run it (fast)**  
1) Detect symmetry (both legs “together”).  
2) Stagger: one leg becomes active barrier/hook, the other becomes pummel/reinsert leg.  
3) Maintain stagger through the first clear attempt.

**DO / DON’T**  
- **DO:** Keep one leg “live” at all times.  
- **DON’T:** Allow both legs to be stapled simultaneously.

**Failure signatures**  
- Both legs stapled → knee line collapses → penetration risk.  
- You lose both lanes at once.

**Metrics**  
- Time spent in “double-controlled legs” state  
- Staple success rate against you

**Links**  
- Upstream: [B-09](#b-09)  
- Downstream: [C-10](#c-10), [C-11](#c-11)

---

<a id="b-11"></a>
### B-11 — Constant Threat Belief OS (Make Them Behave Differently)

**Purpose (plain English)**  
A credible always-on threat changes opponent behavior: they hesitate, reduce commitment, allocate hands to defense, and move more predictably—making your control easier.

**Trigger**  
- Opponent passes with full confidence and constant pressure  
- You need to slow entries and create reaction windows

**Reads**  
- Do they hesitate at all?  
- Do they allocate hands/attention to defense?

**Outputs**  
- Reduced passing commitment + more predictable steps + easier attachment

**Run it (fast)**  
1) Establish a threat that persists across posture changes (standing/kneeling).  
2) Re-assert it repeatedly until they respect it.  
3) Use hesitation to attach and force proof.

**DO / DON’T**  
- **DO:** Choose threats that can’t be turned off by simple posture change.  
- **DON’T:** Rely on conditional threats that disappear when they stand/posture.

**Failure signatures**  
- Opponent never hesitates; you’re stuck reacting forever.  
- Your offense “turns off” when they posture.

**Metrics**  
- Opponent entry attempts per minute (should decrease)  
- Time from hesitation cue → your attachment/entry

**Links**  
- Downstream: [B-12](#b-12), [D-04](#d-04), [D-23](#d-23)

---

<a id="b-12"></a>
### B-12 — Leg Target Selection OS (Posture-Proof Targeting)

**Purpose (plain English)**  
Choose targets that remain available even when the opponent postures or changes stance. Legs are the most posture-proof target class.

**Trigger**  
- Your offense disappears when opponent postures/stands  
- You’re choosing your “primary threat object” for open guard

**Reads**  
- What posture change turns your threat off?  
- Are legs still accessible across those changes?

**Outputs**  
- Target selection: legs as default persistent threat object + a mandate to maintain access

**Run it (fast)**  
1) Identify your current threat’s “off switch.”  
2) If posture/standing kills it, shift primary focus to leg access + distance breaking.  
3) Build your control and conversion around that persistence.

**DO / DON’T**  
- **DO:** Design threats that stay live across stance toggles.  
- **DON’T:** Accept a threat model that opponent can disable with one easy choice.

**Failure signatures**  
- You only threaten when opponent cooperates with posture.  
- Opponent stands and you reset mentally.

**Metrics**  
- Threat persistence across stance changes  
- % engagements where a leg threat is live within first 5 seconds

**Links**  
- Downstream: [B-13](#b-13), [D-03](#d-03), [D-04](#d-04)

<a id="b-13"></a>
### B-13 — Threat Permanence Design OS (Cannot Be Switched Off)

**Purpose (plain English)**  
Ensure your main threat stays live even when the opponent changes posture, stance, or range. If the opponent can disable your threat with one easy toggle, you don’t govern tempo.

**Trigger**  
- Your offense disappears after posture/stance change  
- Opponent repeatedly chooses the same “safe toggle” to turn you off

**Reads**  
- What specific opponent behavior turns your threat off? (stand, hips-back, retreat, angle)  
- Do you have a connector that re-establishes threat under that condition?

**Outputs**  
- A redesigned threat layer that remains live across common toggles

**Run it (fast)**  
1) Identify the “off switch” (the easiest opponent toggle that kills your threat).  
2) Install a connector that makes that toggle costly (reattach + force step map).  
3) Re-test: opponent toggles → threat remains live within 1–2 beats.

**DO / DON’T**  
- **DO:** Build around the opponent’s easiest defense, not your preferred scenario.  
- **DON’T:** Keep a threat model that only works when opponent stays kneeling/close.

**Failure signatures**  
- Same reset pattern keeps occurring.  
- You chase engagement instead of forcing it.

**Metrics**  
- Time from opponent toggle → threat re-established  
- % toggles where threat remains live

**Links**  
- Upstream: [B-11](#b-11), [B-12](#b-12)  
- Downstream: [D-04](#d-04), [D-23](#d-23), [B-08](#b-08)

---

<a id="b-14"></a>
### B-14 — Foot/Ankle Line Control OS (Control vs Touch)

**Purpose (plain English)**  
Prevent “touch-and-lose.” Line control means the leg attachment survives a step and denies easy retraction.

**Trigger**  
- Any time you capture a foot/ankle  
- Opponent immediately retracts/steps to clear

**Reads**  
- Does your hold survive one full opponent step?  
- Can they retract the foot line cleanly?

**Outputs**  
- A leg handle that survives defensive beat #1 and can force a reaction

**Run it (fast)**  
1) Secure the ankle/foot line (not just contact).  
2) Maintain alignment through their first step/turn.  
3) If it slips, treat as failure → replace immediately (tempo).

**DO / DON’T**  
- **DO:** Grade success by “survived one step,” not by “I touched it.”  
- **DON’T:** Upgrade to big actions if line control fails beat #1.

**Failure signatures**  
- You grab ankle, they step, you lose it instantly.  
- You pull without line control and detach.

**Metrics**  
- Contact survival through one opponent step (%)  
- Retraction denial rate

**Links**  
- Downstream: [D-03](#d-03), [D-04](#d-04), [B-06](#b-06)

---

<a id="b-15"></a>
### B-15 — Hips-Connected Attachment OS (Hands + Hips)

**Purpose (plain English)**  
Hands-only control is fragile. Hips-connected attachment denies the opponent’s cheapest escape: separation.

**Trigger**  
- After leg capture  
- During opponent retreat/turn-out to clear  
- Any time you feel stretched long (hands on, hips far)

**Reads**  
- Hip distance to the captured line  
- Can opponent create separation with one retreat step?

**Outputs**  
- “Hands + hips” attachment that survives retreat and turning

**Run it (fast)**  
1) After capture, close hip distance to the attachment line.  
2) Maintain proximity through their first defensive movement.  
3) If hips drift away, re-close immediately before progressing.

**DO / DON’T**  
- **DO:** Treat separation as the enemy; close distance early.  
- **DON’T:** Overextend long-range and get stretched (you’ll lose steering).

**Failure signatures**  
- Hands stay on but opponent retracts cleanly.  
- You get elongated and can’t force reactions.

**Metrics**  
- % captures maintained through opponent retreat/turn  
- “Hip drift” events per round

**Links**  
- Upstream: [B-14](#b-14)  
- Downstream: [D-16](#d-16), [D-17](#d-17), [D-23](#d-23)

---

<a id="b-16"></a>
### B-16 — Sticky Connection Non-Negotiable OS (Beat #1 Survival)

**Purpose (plain English)**  
Any connector (DLR hook, distance breaker, platform entry) is invalid unless connection persists through the opponent’s first defensive beat. This is the universal “entry validity” rule.

**Trigger**  
- Any time you initiate a connector/entry  
- Any time opponent’s first defense is peel/step-away/turn-out

**Reads**  
- Did you maintain at least one meaningful connection through defense beat #1?

**Outputs**  
- VALID connector (survives beat #1) or INVALID connector (collapses)

**Run it (fast)**  
1) Enter connector.  
2) Expect immediate defense.  
3) Maintain one connection through defense beat #1.  
4) Add second connection ASAP ([D-16](#d-16)).  
If you fail beat #1 → treat entry as invalid and restart connection-first.

**DO / DON’T**  
- **DO:** Measure entries by continuity, not by how clean they look.  
- **DON’T:** “Land and lose” then pretend it was progress.

**Failure signatures**  
- You hit entries but detach on first peel and reset neutral.  
- You rely on single-point contact and collapse instantly.

**Metrics**  
- % entries surviving first defensive beat  
- Time to second connection after entry

**Links**  
- Upstream: [B-01](#b-01), [B-06](#b-06)  
- Downstream: [D-16](#d-16), [D-17](#d-17), [A-09](#a-09), [A-10](#a-10)

## Bucket C — Recovery Engines

<a id="c-01"></a>
### C-01 — Knowledge/Denial Micro-Cycle OS (Identify→Deny→Recenter→Reattach→Convert)

**Purpose (plain English)**  
Make defense repeatable. You don’t “defend passes”; you run a cycle that breaks the active requirement and immediately restores alignment + connection, then converts on their repair-step.

**Trigger**  
- Any time the opponent starts building a pass requirement  
- Immediately after any successful denial (cycle continues)  
- Any time you feel “I defended but I’m still losing”

**Reads**  
- Active link (use [A-04](#a-04))  
- `STATE` (NORMAL/ALARM via [A-06](#a-06))  
- Connection status (do you still have a handle?)

**Outputs**  
- Broken active link + restored alignment + reattached handles + a conversion attempt during opponent correction

**Run it (fast)**  
1) **Identify** active link ([A-04](#a-04)).  
2) **Deny** the link (minimal correction, not a scramble).  
3) **Recenter** (re-square alignment) ([C-11](#c-11)).  
4) **Reattach** (restore durable connection + redundancy) ([B-06](#b-06), [B-05](#b-05)).  
5) **Convert** on their repair-step ([D-01](#d-01)).

**DO / DON’T**  
- **DO:** Complete the cycle; denial alone is incomplete defense.  
- **DON’T:** Deny and pause (opponent rebuilds immediately).

**Failure signatures**  
- “Win the moment, lose the next step.”  
- Deny grips but stay rotated (angle persists).  
- Survive pressure but remain leg-late.

**Metrics**  
- Cycle completion rate (did you reach reattach + convert?)  
- Deny→recenter latency (beats)  
- Conversions initiated during repair-step (%)

**Links**  
- Upstream: [A-04](#a-04), [A-06](#a-06)  
- Downstream: [C-09](#c-09), [D-01](#d-01)

---

<a id="c-02"></a>
### C-02 — Demarcation Theory OS (Name the First Line You’re Losing)

**Purpose (plain English)**  
Stop random scrambling. Identify *where* guard is failing first (the earliest line/zone) so you choose the correct recovery tool.

**Trigger**  
- Guard feels “slippery” / alignment drifting  
- Opponent is gaining angle/level/entry depth and you’re unsure what to do

**Reads (demarcation lines — earliest matters most)**  
- **Distance line:** are you losing space too easily?  
- **Knee line:** are your legs being cleared/stapled so reinsertion is failing?  
- **Hip line:** is opponent entering past your primary barriers / about to pin?  
- **Shoulder line:** are you being turned/flattened so you can’t face them?

**Outputs**  
- One declared “first failing line” + correct tool family selection

**Run it (fast)**  
1) Ask: “What line failed first?”  
2) Fix that earliest line with the smallest tool.  
3) Re-test immediately (line-loss shifts after correction).

**DO / DON’T**  
- **DO:** Fix the earliest line-loss first; upstream repairs collapse downstream threats.  
- **DON’T:** Fight late symptoms while early failure persists.

**Failure signatures**  
- You recover once, then same failure repeats instantly.  
- You fix grips but angle/shoulder line keeps losing.

**Metrics**  
- Time from first line-loss cue → corrective action  
- Repeat-failure frequency (same line failing repeatedly)

**Links**  
- Downstream: [C-03 Router](#c-03), [A-06 Alarm Gate](#a-06)

---

<a id="c-03"></a>
### C-03 — Demarcation-to-Tool Router OS (One Problem → One Tool)

**Purpose (plain English)**  
Convert diagnosis into action. This router maps the failing line + `STATE` into the correct tool family, without chaining random movements.

**Trigger**  
- Immediately after [C-02](#c-02)  
- Any time you hesitate between multiple recoveries

**Inputs**  
- Failing line (distance/knee/hip/shoulder)  
- `STATE` from [A-06](#a-06)

**Outputs**  
- One selected recovery tool family + the required terminal step

**Routing rules (fast)**
- If `STATE: ALARM` → structure-first tools ([C-06](#c-06)→[C-07](#c-07)→[C-08](#c-08)) then **terminal reinsertion** ([C-15](#c-15)).  
- If `STATE: NORMAL` → mobility-first tools (re-square + reinsertion) ([C-11](#c-11)→[C-10](#c-10)).

**Run it (fast)**  
1) Determine `STATE`.  
2) Select tool family (structure-first vs mobility-first).  
3) Execute one tool.  
4) Finish with terminal step: legs-in + attach (see [C-15](#c-15) + [B-06](#b-06)).

**DO / DON’T**  
- **DO:** One tool → reassess.  
- **DON’T:** Stack 4 movements without diagnosis.

**Failure signatures**  
- Scramble chains that worsen alignment.  
- You select mobility tools while compressed (pin follows).

**Metrics**  
- “One tool” compliance rate  
- Scramble-to-pin frequency

**Links**  
- Upstream: [C-02](#c-02), [A-06](#a-06)  
- Downstream: [C-09](#c-09)

---

<a id="c-04"></a>
### C-04 — Essential Movement Selector OS (Minimal Correction First)

**Purpose (plain English)**  
Choose the smallest movement that restores the failing line. Escalate only if it fails. This prevents over-rotation and self-created exposure.

**Trigger**  
- You know the problem (line-loss) but feel tempted to “do a big escape”  
- You’re under pressure and need a safe default

**Reads**  
- Space availability (do you have room?)  
- Which line is failing (distance/knee/hip/shoulder)

**Outputs**  
- One chosen movement (not a combo) that restores the line

**Run it (fast)**  
1) Pick the smallest movement that restores the earliest failing line.  
2) Execute once with intent.  
3) Reassess. If unresolved, escalate to the next larger tool.

**DO / DON’T**  
- **DO:** Make minimal corrections repeatable under fatigue.  
- **DON’T:** Over-rotate (you donate angle and shoulder line).

**Failure signatures**  
- You create your own exposure by moving too much.  
- Big movements that don’t end with legs-in.

**Metrics**  
- Over-rotation events per round  
- Tool selection speed under pressure

**Links**  
- Downstream: [C-11](#c-11), [C-10](#c-10), [C-09](#c-09)

<a id="c-05"></a>
### C-05 — Mobility-First Retention OS (`STATE: NORMAL`)

**Purpose (plain English)**  
When hip-line danger is not present, mobility solves faster than heavy framing. This OS prioritizes re-square + reinsertion before the passer accumulates angle.

**Trigger**  
- [A-06](#a-06) declares `STATE: NORMAL`  
- You have space to move and re-square

**Reads**  
- Angle drift beginning (opponent circling)  
- Lane status (are your legs between you and them?)

**Outputs**  
- Front-facing alignment restored + legs reinserted + distance line rebuilt

**Run it (fast)**  
1) **Re-square** ([C-11](#c-11)).  
2) **Reinsert lanes** ([C-10](#c-10)).  
3) **Reattach** handles + redundancy ([B-06](#b-06), [B-05](#b-05)).  
4) **Convert** on their repair-step ([D-01](#d-01)).

**DO / DON’T**  
- **DO:** Move first; frame only if alarm flips ON.  
- **DON’T:** Frame early and stall vs mobility (you’ll get run around).

**Failure signatures**  
- Early frames → angle loss.  
- You move but never get legs back in front.

**Metrics**  
- Time from drift cue → re-square  
- % NORMAL threats solved without switching to ALARM

**Links**  
- Upstream: [A-06](#a-06), [A-08](#a-08)  
- Downstream: [C-11](#c-11), [C-10](#c-10), [C-12](#c-12)

---

<a id="c-06"></a>
### C-06 — Defensive Framework Activation OS (`STATE: ALARM`)

**Purpose (plain English)**  
When hip-line danger is present, structure must come before mobility. Frames/wedges create a space budget that you spend to rebuild legs-in position.

**Trigger**  
- [A-06](#a-06) declares `STATE: ALARM`  
- Compression is stable; pin mechanics forming

**Reads**  
- Where pressure is entering (hip line / shoulder line)  
- Frame integrity (are you pushing or wedging?)

**Outputs**  
- Load-bearing structure that halts penetration long enough to realign + reinsert legs

**Run it (fast)**  
1) Build wedges/frames aligned with pressure (no pushing).  
2) Protect shoulder line (don’t get turned flat).  
3) Create a window (usable space).  
4) Transition to recovery sequencing ([C-09](#c-09)) and terminal reinsertion ([C-15](#c-15)).

**DO / DON’T**  
- **DO:** Let frames buy time; legs spend it.  
- **DON’T:** Try fancy mobility while compressed (pin completes).

**Failure signatures**  
- Arms burn out (pushing).  
- You “move” but get flattened because structure wasn’t installed.

**Metrics**  
- Alarm-on → stable structure time  
- % ALARM events resolved without pin

**Links**  
- Upstream: [A-06](#a-06)  
- Downstream: [C-07](#c-07), [C-08](#c-08), [C-09](#c-09), [C-15](#c-15)

---

<a id="c-07"></a>
### C-07 — Frame Integrity OS (Wedge, Don’t Bench Press)

**Purpose (plain English)**  
Frames must be skeletal wedges that carry load. Pushing is fatigue + collapse. This OS keeps your structure functional under pressure.

**Trigger**  
- Any time you are framing under load  
- Especially during `STATE: ALARM`

**Reads**  
- Is your frame aligned with pressure (wedge) or extended away (push)?  
- Are your frames collapsing as opponent settles weight?

**Outputs**  
- Frames that hold shape long enough to reinsert legs

**Run it (fast)**  
1) Set frame as a wedge aligned with incoming pressure.  
2) Maintain shape; avoid extension battles.  
3) Use the time to move hips/legs into reinsertion.

**DO / DON’T**  
- **DO:** Reset frame shape immediately if it starts to fold.  
- **DON’T:** Push harder when losing shape (you’ll gas and still lose).

**Failure signatures**  
- Fast arm fatigue.  
- Frame “exists” but doesn’t stop pressure line.

**Metrics**  
- Frame hold time under load  
- Collapse events per round

**Links**  
- Upstream: [C-06](#c-06)  
- Downstream: [C-08](#c-08), [C-15](#c-15)

---

<a id="c-08"></a>
### C-08 — Compression Management OS (Space Budgeting)

**Purpose (plain English)**  
Space is a budget: preserve it, then spend it immediately to rebuild guard. If you gain space and don’t reinsert/realign, it disappears.

**Trigger**  
- Opponent compresses distance  
- You create a pocket of space (even small)

**Reads**  
- Usable space present? (yes/no)  
- Is opponent “following” to re-collapse immediately?

**Outputs**  
- Space preserved long enough to realign + reinsert legs + reattach handles

**Run it (fast)**  
1) Preserve space with wedges/frames ([C-07](#c-07)).  
2) Align (re-square) as soon as you can ([C-11](#c-11)).  
3) Reinsert legs ([C-10](#c-10) → [C-15](#c-15)).  
4) Reattach handles ([B-06](#b-06)).

**DO / DON’T**  
- **DO:** Spend space immediately on legs-in.  
- **DON’T:** Pause in the opening; opponent re-collapses.

**Failure signatures**  
- You make space, then get re-smashed instantly.  
- You survive but remain leg-late.

**Metrics**  
- Re-collapse frequency after initial space creation  
- Time from space creation → legs-in completion

**Links**  
- Downstream: [C-09 Sequencing](#c-09)

<a id="c-09"></a>
### C-09 — Recovery Sequencing OS (Space→Align→Reinsert→Attach)

**Purpose (plain English)**  
Make recoveries stick. This order converts “escape moments” into restored guard function. Skipping steps is why recoveries fail immediately.

**Trigger**  
- After any denial/movement/frame that creates space  
- Any time you feel “I escaped but I’m still losing”

**Reads**  
- Space availability (usable or collapsing)  
- Alignment status (square or rotated)  
- Leg position (in front or late)

**Outputs**  
- Functional guard restored: legs-in + alignment + at least one handle

**Non-negotiable order**
1) **Space** (create/preserve)  
2) **Align** (re-square hips/shoulders)  
3) **Reinsert** (legs back between you and them)  
4) **Attach** (handles + redundancy)

**Run it (fast)**  
1) Secure a pocket of space ([C-07](#c-07), [C-08](#c-08)).  
2) Re-square ([C-11](#c-11)).  
3) Reinsert legs ([C-10](#c-10), [C-15](#c-15)).  
4) Reattach immediately ([B-06](#b-06), [B-05](#b-05)).

**DO / DON’T**  
- **DO:** Treat “Attach” as the finish line, not “I moved.”  
- **DON’T:** Reinsert while misaligned (you build crooked guard).

**Failure signatures**  
- You shrimp/scoot but don’t reinsert → re-collapse.  
- You reinsert but remain rotated → angle persists.

**Metrics**  
- % recoveries ending with legs-in + handle  
- Space creation → reinsertion completion time

**Links**  
- Upstream: [C-08](#c-08)  
- Downstream: [B-06](#b-06), [D-01](#d-01)

---

<a id="c-10"></a>
### C-10 — Continuous Reinsertion OS (Legs Never Stay Late)

**Purpose (plain English)**  
If legs are late, defense is late. Reinsertion must be continuous during the exchange, not an occasional “big reset.”

**Trigger**  
- Any leg clear/staple/scoop attempt  
- Any time inside lanes are lost  
- Any time you’re framing but legs are not returning

**Reads**  
- Which leg/lane is late  
- Can you reinsert immediately or is `STATE: ALARM` forcing structure-first?

**Outputs**  
- Legs returned to functional lanes + barrier restored

**Run it (fast)**  
1) Identify the late leg.  
2) Reinsert immediately (smallest correction first).  
3) Repeat continuously until inside lanes are stable.

**DO / DON’T**  
- **DO:** Use frames to buy time specifically for reinsertion.  
- **DON’T:** Hand-fight while legs stay cleared.

**Failure signatures**  
- You “survive” with frames but never rebuild legs-in.  
- Knee line opens and penetration follows.

**Metrics**  
- Average “leg-late time” per round  
- Knee-line collapse events per round

**Links**  
- Upstream: [A-06](#a-06)  
- Downstream: [C-15](#c-15), [B-09](#b-09)

---

<a id="c-11"></a>
### C-11 — Immediate Re-Square OS (Angle Kills Early)

**Purpose (plain English)**  
Angle is the early killer. If you re-square early, you avoid hip-line danger. If you re-square late, you pay with ALARM compression.

**Trigger**  
- Opponent circles/redirects  
- You feel hip rotation drifting away from square  
- You are about to “reach with hands” to track them

**Reads**  
- Are they moving off-center (flank/hip line)?  
- Are your hips/shoulders still facing them?

**Outputs**  
- Front-facing alignment restored

**Run it (fast)**  
1) Re-square using hips/feet (not reaching).  
2) Reinsert lanes immediately ([C-10](#c-10)).  
3) Reattach and resume step-map control.

**DO / DON’T**  
- **DO:** Fix angle early; it’s cheap.  
- **DON’T:** Chase with hands while hips lag.

**Failure signatures**  
- You chase shoulders but still get flanked.  
- Angle snowballs into ALARM.

**Metrics**  
- Circle begins → square restored time  
- Angle-loss events per round

**Links**  
- Upstream: [A-02 Energy Read](#a-02)  
- Downstream: [C-10](#c-10), [C-12](#c-12), [B-08](#b-08)

---

<a id="c-12"></a>
### C-12 — Mobility Defense Loop OS (Feet + Re-Square + Reinsert)

**Purpose (plain English)**  
A repeatable loop vs mobility passers: keep them in front by maintaining feet connection, enforcing asymmetry, and re-squaring immediately.

**Trigger**  
- [A-08](#a-08) declares `ARCHETYPE: MOBILITY`  
- Any time opponent attempts to circle/run around

**Reads**  
- Feet-on-them status  
- Angle drift status  
- Leg symmetry status

**Outputs**  
- Opponent kept front-facing; angle accumulation denied; proof windows created

**Run it (loop)**
1) Feet contact ON ([B-09](#b-09)).  
2) Create/maintain asymmetry ([B-10](#b-10)).  
3) Re-square immediately ([C-11](#c-11)).  
4) Reinsert lanes ([C-10](#c-10)).  
5) Resume steering to force steps ([B-08](#b-08)).  
Repeat until a repair-step window appears ([D-01](#d-01)).

**DO / DON’T**  
- **DO:** KPI = “they stay in front.”  
- **DON’T:** Freeze and frame; mobility punishes stalling with angle.

**Failure signatures**  
- Free circles; you chase late.  
- You lose inside lanes while focused on hand-fighting.

**Metrics**  
- % time opponent remains in front  
- Angle-loss events per round  
- Forced steps/posts per minute (from step-map control)

**Links**  
- Upstream: [A-08](#a-08)  
- Downstream: [D-01](#d-01), [D-23](#d-23)

<a id="c-13"></a>
### C-13 — Pressure Defense Ladder OS (Early Deny → Structure → Reinsert)

**Purpose (plain English)**  
A two-phase response for pressure passers: stop the lock early; if late, survive compression and rebuild guard. Prevents “accept lock then panic.”

**Trigger**  
- [A-08](#a-08) declares `ARCHETYPE: PRESSURE`  
- Opponent closes distance and begins clamp/lock mechanics

**Reads**  
- Phase: **EARLY** (lock not stable yet) vs **LATE** (compression/lock stable)  
- `STATE` from [A-06](#a-06)

**Outputs**  
- EARLY: lock prevented/broken before stable compression  
- LATE: compression survived + legs reinserted + return to NORMAL

**Run it (fast)**
- **EARLY phase**
  1) Deny distance collapse and connection-building ([C-14](#c-14)).  
  2) Re-square + reinsert lanes ([C-11](#c-11), [C-10](#c-10)).  
  3) Reattach and force step windows ([B-06](#b-06), [B-08](#b-08)).
- **LATE phase**
  1) Framework activation (wedges/frames) ([C-06](#c-06), [C-07](#c-07)).  
  2) Space budgeting ([C-08](#c-08)).  
  3) Sequencing Space→Align→Reinsert→Attach ([C-09](#c-09)).  
  4) Terminal step: legs-in ([C-15](#c-15)).

**DO / DON’T**  
- **DO:** Treat EARLY denial as the cheapest win.  
- **DON’T:** Try mobility solutions inside stable compression (pin completes).

**Failure signatures**  
- You allow lock, then spend the round in ALARM survival.  
- You escape once but never reinsert legs; they re-lock immediately.

**Metrics**  
- Lock denied before stable compression (%)  
- Pins occurring after pressure sequences  
- % defenses ending with legs-in + handle

**Links**  
- Upstream: [A-08](#a-08), [A-06](#a-06)  
- Downstream: [C-14](#c-14), [C-15](#c-15)

---

<a id="c-14"></a>
### C-14 — Lock Formation Early-Denial OS (Stop the Clamp Before It Stabilizes)

**Purpose (plain English)**  
Pressure passing becomes hard to stop once the lock is stable. This OS attacks the lock while it’s still forming—before compression becomes a pin.

**Trigger**  
- First contact of a pressure sequence  
- Hands/arms seeking clamps, head/shoulder pinning, chest-to-hip glue attempts

**Reads (early lock cues)**  
- Connecting hands / underhook-style clamps forming  
- Head positioning that turns you away  
- Chest-to-hip closure (space disappearing)  
- Your legs being stapled/cleared while they settle weight

**Outputs**  
- Lock prevented or broken + barriers re-established

**Run it (fast)**  
1) Deny the *closing action* (don’t allow chest/hips to glue).  
2) Break the lock structure (not just one grip—break the mechanism).  
3) Re-square and reinsert lanes immediately.  
4) Reattach and resume step-map control.

**DO / DON’T**  
- **DO:** Start denial on the first lock cue, not after you feel crushed.  
- **DON’T:** “Hand fight” without rebuilding legs-in barriers.

**Failure signatures**  
- You defend grips but lock structure remains.  
- You wait until compression is stable, then you’re forced into ALARM.

**Metrics**  
- Time lock cue → disruption  
- % pressure sequences stopped before stable compression

**Links**  
- Upstream: [A-03](#a-03) (where in chain are they?)  
- Downstream: [C-11](#c-11), [C-10](#c-10), [C-13](#c-13)

---

<a id="c-15"></a>
### C-15 — Leg Reinsertion Terminal Step OS (Every Defense Ends Legs-In)

**Purpose (plain English)**  
Defense is incomplete until legs are back between you and them. This is the “finish line” for all recoveries.

**Trigger**  
- After any successful wedge/frame/denial/movement  
- Any time you feel “I survived” but you’re still leg-late

**Reads**  
- Barrier status: legs-in vs legs-cleared

**Outputs**  
- Playable guard restored: legs-in + alignment + at least one handle

**Run it (fast)**  
1) Ensure space exists (even small) ([C-08](#c-08)).  
2) Align (re-square) ([C-11](#c-11)).  
3) Reinsert legs (inside lanes restored) ([C-10](#c-10)).  
4) Attach (durable handle + redundancy) ([B-06](#b-06), [B-05](#b-05)).

**DO / DON’T**  
- **DO:** Treat legs-in as non-negotiable completion.  
- **DON’T:** Pause at “survival” while legs stay late.

**Failure signatures**  
- You frame forever and still get passed.  
- You escape but get re-collapsed instantly (no terminal step).

**Metrics**  
- % defenses ending legs-in within 2–3 beats  
- Re-collapse events after “successful defense”

**Links**  
- Downstream: [B-06](#b-06), [B-08](#b-08), [D-01](#d-01)

## Bucket D — Conversion Engines

<a id="d-01"></a>
### D-01 — Repair-Step Window OS (Convert During Their Fix)

**Purpose (plain English)**  
The highest-yield conversion moment is when the opponent must repair base/posture after you disrupt them. Convert *during* the repair step, not after stability returns.

**Trigger**  
- You force a step/post/posture correction (see [B-03](#b-03), [B-08](#b-08), [C-01](#c-01))  
- Opponent visibly “fixes” feet or posture

**Reads**  
- Is the opponent currently transitioning (foot in air, hands posting, posture rebuilding)?  
- Is the window still open (before they plant and stabilize)?

**Outputs**  
- Conversion initiated before re-stabilization: entry, platform, consolidation, or anti-exit follow

**Run it (fast)**  
1) Cause disruption (deny link / steer base).  
2) See repair-step start (transition cue).  
3) Convert immediately (commit while they are reorganizing).  
4) If window closes, don’t force—recreate proof.

**DO / DON’T**  
- **DO:** Treat “foot in air / hands posting” as permission slips.  
- **DON’T:** Admire your disruption and then attack a stable base.

**Failure signatures**  
- You generate reactions but gain no ground.  
- Opponent repairs cleanly and restarts passing with confidence.

**Metrics**  
- Disruption → conversion latency (beats)  
- % conversions initiated before stance stabilizes

**Links**  
- Upstream: [B-03](#b-03), [B-08](#b-08), [C-01](#c-01)  
- Downstream: [D-05](#d-05), [D-11](#d-11), [D-16](#d-16), [D-23](#d-23)

---

<a id="d-02"></a>
### D-02 — Reaction Window Conversion System (Force → Convert)

**Purpose (plain English)**  
Reactions are temporary. This system enforces: if you forced the reaction, you must convert inside the reaction window or you must recreate it.

**Trigger**  
- Any forced step/post/posture change (especially within 1–2 beats)

**Reads**  
- Which reaction occurred: step vs post vs posture shift  
- Is connection still sticky through beat #1? ([B-16](#b-16))

**Outputs**  
- Immediate upgrade: deeper attachment, entry initiation, or consolidation installation

**Run it (fast)**  
1) Force reaction ([B-03](#b-03)).  
2) Convert within 1–2 beats (entry/upgrade/stabilize).  
3) Install second connection immediately ([D-16](#d-16)).  
4) If missed, restart steering to force a new reaction.

**DO / DON’T**  
- **DO:** Convert while they are reacting, not after they stabilize.  
- **DON’T:** Force reaction and pause (that’s gifting the repair).

**Failure signatures**  
- Reaction happens; you hesitate; opponent repairs and strips.  
- You convert without sticky connection and lose everything on first peel.

**Metrics**  
- Reaction → conversion time  
- % reactions producing tangible progress (entry/control)

**Links**  
- Upstream: [B-03](#b-03)  
- Downstream: [D-16](#d-16), [D-17](#d-17), [D-23](#d-23)

---

<a id="d-03"></a>
### D-03 — 2-on-1 Ankle Primary Tool OS (Standing Handle)

**Purpose (plain English)**  
A reliable standing conversion tool: create a posture-proof leg handle that forces immediate base reactions and anchors your entry chains.

**Trigger**  
- `REGIME: STANDING` and you can access foot/ankle line  
- Opponent is retreating or stable and you need a high-leverage handle

**Reads**  
- Can you secure true line control (survive one step)? ([B-14](#b-14))  
- Is opponent toes-loaded vs heels-loaded? ([A-01b](#a-01b))

**Outputs**  
- Durable ankle handle that forces step/turn/post within 1–2 beats

**Run it (fast)**  
1) Establish true 2-on-1 control on ankle/foot line.  
2) Apply direction to force reaction (step/turn/post).  
3) Convert on the reaction window ([D-01](#d-01)).  
4) If they retract/peel, replace immediately ([B-06](#b-06)).

**DO / DON’T**  
- **DO:** Grade it by “survives one step + forces reaction.”  
- **DON’T:** Treat a touch as control.

**Failure signatures**  
- You grab ankle; they step away; contact breaks.  
- You pull without direction; no reaction.

**Metrics**  
- Reaction rate within 1–2 beats  
- Contact survival through one step  
- Conversion rate after first reaction

**Links**  
- Upstream: [B-14](#b-14), [B-15](#b-15)  
- Downstream: [D-04](#d-04), [D-16](#d-16), [D-23](#d-23)

---

<a id="d-04"></a>
### D-04 — Distance Breaker OS (Outside-Range Conversion)

**Purpose (plain English)**  
Solve the “they won’t engage” problem. Convert outside range into immediate attachment, without waiting for them to commit.

**Trigger**  
- Opponent stalls just outside your attachment range  
- Repeated disengage resets (`ENERGY: WITHDRAW`)  
- You need to bridge range into leg contact

**Reads**  
- Can you maintain sticky connection through defense beat #1? ([B-16](#b-16))  
- Is opponent retreating or stepping in?

**Outputs**  
- Immediate attachment that survives beat #1 + rapid redundancy install

**Run it (fast)**  
1) Initiate distance breaker to close range.  
2) Prioritize attachment before/at peak extension.  
3) Accept imperfect landing; grade success by continuity (beat #1 survival).  
4) Install second connection immediately ([D-16](#d-16)) and convert.

**DO / DON’T**  
- **DO:** Measure success by “connected after landing,” not aesthetics.  
- **DON’T:** Throw entries that detach instantly.

**Failure signatures**  
- You “enter” but lose the leg on first peel.  
- You wait for engagement and nothing happens.

**Metrics**  
- Outside-range → first attachment time  
- Beat #1 survival rate  
- Resets prevented per round

**Links**  
- Upstream: [A-02](#a-02) (WITHDRAW)  
- Downstream: [D-16](#d-16), [D-23](#d-23), [B-06](#b-06)

<a id="d-05"></a>
### D-05 — Kneeling Entry Decision OS (Choose Family Only When Base Is Committable)

**Purpose (plain English)**  
Select the correct kneeling entry family only when the kneeling base is actually compromisable. Prevents “hope shots” into stable kneeling posture.

**Trigger**  
- `REGIME: KNEELING`  
- You want to enter (single / double / reverse double)

**Reads**  
- Kneeling posture reality via [A-01a](#a-01a): shoulders-leading vs hips-stacked  
- Proof presence (post/step/collapse) via [D-06](#d-06)  
- Leg availability (one leg realistically available vs two)

**Outputs**  
- Entry family selection: SINGLE / DOUBLE / REVERSE DOUBLE  
- “ENTER NOW” vs “CREATE PROOF FIRST”

**Run it (fast)**  
1) Call kneeling posture: shoulders-leading or hips-stacked ([A-01a](#a-01a)).  
2) Demand proof (post/step/collapse) ([D-06](#d-06)).  
3) Choose family:
   - One leg available → [D-07](#d-07)  
   - Two legs available → [D-08](#d-08)  
   - Standard alignment denied but proof exists → [D-09](#d-09)  
4) After entry contact, immediately bridge to consolidation ([D-17](#d-17)).

**DO / DON’T**  
- **DO:** Treat proof as permission to commit.  
- **DON’T:** Force double when only one leg exists.

**Failure signatures**  
- Entries get stuffed “mysteriously” (usually no proof).  
- Touch leg then lose it immediately (no consolidation).

**Metrics**  
- % kneeling entries initiated on proof  
- Entry-to-control conversion rate

**Links**  
- Upstream: [A-01a](#a-01a), [D-01](#d-01)  
- Downstream: [D-06](#d-06), [D-07](#d-07), [D-08](#d-08), [D-09](#d-09), [D-17](#d-17)

---

<a id="d-06"></a>
### D-06 — Proof-Gated Entry OS (Kneeling Permission Slip)

**Purpose (plain English)**  
Proof prevents hope. No proof = no entry. Proof is the observable base compromise that makes the entry high percentage.

**Trigger**  
- You are “close enough” to enter but base looks stable  
- You’re about to commit under kneeling posture

**Reads (proof signals)**  
- Hand **post** appears  
- A **step** to repair balance  
- Visible **collapse** forward/side  
- Weight commitment that forces a correction

**Outputs**  
- ALLOW entry vs DENY entry (create proof first)

**Run it (fast)**  
1) If proof absent → steer/deny until proof appears (force step/post).  
2) When proof appears → enter immediately (window is short).  
3) After contact, install second connection and consolidate.

**DO / DON’T**  
- **DO:** Enter within 1–2 beats of proof.  
- **DON’T:** Wait after proof; it evaporates when they re-stabilize.

**Failure signatures**  
- You attempt entries into stable kneeling base and get stalled.  
- You see proof but delay, then complain it “didn’t work.”

**Metrics**  
- Invalid entry attempts per round  
- Proof→entry initiation latency (beats)

**Links**  
- Upstream: [B-03](#b-03) (force reactions), [D-01](#d-01)  
- Downstream: [D-07](#d-07), [D-08](#d-08), [D-09](#d-09), [D-16](#d-16)

---

<a id="d-07"></a>
### D-07 — Single-Leg Entry System OS (Kneeling Primary When One Leg Is Real)

**Purpose (plain English)**  
High-reliability kneeling entry when only one leg is realistically capturable. Optimized for “touch → secure → stabilize” without donating separation.

**Trigger**  
- Proof present ([D-06](#d-06))  
- Only one leg is truly available (the other is hidden/posted/too far)

**Reads**  
- Can you secure the leg line through defense beat #1? ([B-16](#b-16))  
- Can you keep hips connected to prevent retraction? ([B-15](#b-15))

**Outputs**  
- Secure single-leg access that immediately bridges to consolidation

**Run it (fast)**  
1) Initiate on proof (no proof = no entry).  
2) Secure leg line (control, not touch).  
3) Install second connection within 1–2 beats ([D-16](#d-16)).  
4) Bridge to consolidation ([D-17](#d-17)).

**DO / DON’T**  
- **DO:** Treat “secure + second connection” as the entry completion.  
- **DON’T:** Enter and then scramble without control.

**Failure signatures**  
- Touch leg, opponent retracts, you reset.  
- You lose connection on first peel.

**Metrics**  
- Entry→second connection time  
- First-peel survival rate  
- Entry→consolidation time

**Links**  
- Downstream: [D-16](#d-16), [D-17](#d-17), [D-20](#d-20)

---

<a id="d-08"></a>
### D-08 — Double-Leg Entry System OS (Kneeling When Both Legs Are Capturable)

**Purpose (plain English)**  
Use when proof indicates a split/forward commitment that exposes both legs. Designed to prevent pivot/turn-out during initiation.

**Trigger**  
- Proof present  
- Both legs are realistically capturable (not theoretical)

**Reads**  
- Are both knees/legs within capture range simultaneously?  
- Is opponent about to turn-out or retreat?

**Outputs**  
- Two-leg capture that transitions directly into stabilization (knee-line containment + consolidation)

**Run it (fast)**  
1) Enter on proof.  
2) Capture both legs (deny immediate retract).  
3) Stabilize knee line early ([D-20](#d-20)).  
4) Install second connection redundancy ([D-16](#d-16)) and consolidate ([D-17](#d-17)).

**DO / DON’T**  
- **DO:** If both legs aren’t truly there, downgrade to single immediately.  
- **DON’T:** Sacrifice connection for speed; you’ll get pivoted off.

**Failure signatures**  
- Forced double when only one leg existed.  
- Opponent pivots/turns out during loose capture.

**Metrics**  
- % doubles reaching knee-line stabilization  
- Turn-out escapes during initiation

**Links**  
- Downstream: [D-20](#d-20), [D-16](#d-16), [D-17](#d-17)

---

<a id="d-09"></a>
### D-09 — Reverse Double-Leg Entry System OS (When Standard Alignment Is Denied)

**Purpose (plain English)**  
A double-leg family for when conventional alignment is blocked but proof exists. Uses reverse orientation to maintain access without losing continuity.

**Trigger**  
- Proof present  
- Standard double entry alignment is denied (angle/frames prevent it)  
- Reverse alignment allows access without separation

**Reads**  
- Will reverse orientation preserve connection through defense beat #1? ([B-16](#b-16))  
- Does reverse create distance or maintain hip connection?

**Outputs**  
- Reverse entry that keeps attachment and routes to consolidation

**Run it (fast)**  
1) Enter on proof with reverse alignment.  
2) Maintain at least one connection through first defensive beat.  
3) Install second connection immediately ([D-16](#d-16)).  
4) Bridge to consolidation ([D-17](#d-17)).

**DO / DON’T**  
- **DO:** Abort if reverse creates separation; re-create proof instead.  
- **DON’T:** “Spin” without attachment (that’s just giving distance).

**Failure signatures**  
- Reverse entry produces distance; opponent resets.  
- You rotate but lose the legs.

**Metrics**  
- Beat #1 survival rate for reverse entries  
- Reverse entry → consolidation rate

**Links**  
- Downstream: [D-16](#d-16), [D-17](#d-17)

<a id="d-10"></a>
### D-10 — Bridge-Platform Integration OS (X / RDLR / HQ Are Routing Platforms)

**Purpose (plain English)**  
Platforms are not destinations. Their job is to (1) survive beat #1, (2) force a reaction, (3) route you into stabilization/hub selection that denies the opponent’s best exit.

**Trigger**  
- You establish X / RDLR / HQ  
- You land in a platform from a scramble  
- You’re tempted to “hang out” in platform control

**Reads**  
- Platform validity (proof + restriction + beat #1 survival) via [A-09](#a-09) + [B-16](#b-16)  
- Opponent’s first response: drive / turn / retreat / peel

**Outputs**  
- Platform stabilized (briefly) → reaction forced → routed to consolidation/hub

**Run it (fast)**  
1) Confirm platform is valid (survive beat #1).  
2) Install second connection immediately ([D-16](#d-16)).  
3) Force a reaction (step/turn/post) ([B-03](#b-03)).  
4) Route to hub/stabilization that blocks their exit ([D-21](#d-21), [D-23](#d-23)).

**DO / DON’T**  
- **DO:** Keep platform time short; it exists to produce a routed outcome.  
- **DON’T:** Attack without suppressing the primary exit.

**Failure signatures**  
- Stall in platform → peel clears → full reset.  
- You attack while exit is live → opponent resets (backstep/flee/turn-away).

**Metrics**  
- Platform→hub conversion rate  
- Time platform established → first forced reaction

**Links**  
- Upstream: [A-09](#a-09), [B-16](#b-16)  
- Downstream: [D-11](#d-11), [D-21](#d-21), [D-23](#d-23)

---

<a id="d-11"></a>
### D-11 — Momentum Entry OS (Enter on Motion, Not on Stability)

**Purpose (plain English)**  
Static bases stuff entries. Motion creates openings. This OS makes you time entries on steps, turns, retreats, and repair-steps.

**Trigger**  
- Opponent is stepping/turning/retreating  
- Immediately after you force a reaction ([B-03](#b-03))  
- During repair-step windows ([D-01](#d-01))

**Reads**  
- Motion type: step / turn / retreat / post  
- Are you connected enough to survive beat #1? ([B-16](#b-16))

**Outputs**  
- Entry/upgrade initiated inside the transition window

**Run it (fast)**  
1) Identify motion.  
2) Enter/upgrade during the transition.  
3) Add redundancy immediately; route to stabilization.

**DO / DON’T**  
- **DO:** If base is stable, create motion first (step map).  
- **DON’T:** Shoot into stable posture and expect it to work.

**Failure signatures**  
- Stuffed entries into stable base.  
- Hesitation after reaction; window closes.

**Metrics**  
- % entries initiated during motion (vs static)  
- Stuffed-entry rate

**Links**  
- Upstream: [B-08](#b-08), [D-01](#d-01)  
- Downstream: [D-16](#d-16), [D-17](#d-17)

---

<a id="d-12"></a>
### D-12 — X-Guard Triple-Attack Router OS (Response-Based Lane Selection)

**Purpose (plain English)**  
From X, you choose the lane that punishes the opponent’s first response. Prevents predictable “same attack every time.”

**Trigger**  
- X platform established and opponent reacts

**Reads**  
- Opponent response: **DRIVE** / **TURN** / **RETREAT**  
- Load status: do you have their weight captured enough to off-balance?

**Outputs**  
- Correct lane selection (one primary lane, not three at once)

**Run it (fast)**  
1) Force/observe the first reaction.  
2) Select the lane that punishes that reaction.  
3) Stabilize if exit is live; finish only after suppression ([D-27](#d-27)).

**DO / DON’T**  
- **DO:** Demand load before you try to turn/off-balance.  
- **DON’T:** Spam the same lane regardless of response.

**Failure signatures**  
- Step-out escapes because you turned without load.  
- Predictability: opponent pre-defends.

**Metrics**  
- Correct lane selection rate  
- Step-out/escape frequency after initiating attack

**Links**  
- Downstream: [D-21](#d-21), [D-23](#d-23), [D-27](#d-27)

---

<a id="d-13"></a>
### D-13 — RDLR as Anti-Pressure Bridge OS (Survive → Convert, Not Hang On)

**Purpose (plain English)**  
Use RDLR to absorb pressure without giving clean disengagement. The goal is to force proof windows and route into stabilization, not to stall.

**Trigger**  
- `ARCHETYPE: PRESSURE` closes distance  
- You need a bridge platform that keeps connection under compression

**Reads**  
- Can you maintain sticky attachment through beat #1? ([B-16](#b-16))  
- Is opponent trying to peel/clear and reset?

**Outputs**  
- Pressure absorbed → connection maintained → proof window appears → route to hub

**Run it (fast)**  
1) Maintain attachment through the first pressure beat.  
2) Deny angle/run-around while under pressure.  
3) Create proof via their corrective steps.  
4) Route to hub based on exit attempt ([D-21](#d-21), [D-23](#d-23)).

**DO / DON’T**  
- **DO:** Treat RDLR as a bridge to conversion.  
- **DON’T:** Allow free step-away; reattach before continuing.

**Failure signatures**  
- RDLR contact exists but does not restrict; peel clears and opponent resets.  
- You stall and get flattened.

**Metrics**  
- RDLR survival→conversion rate  
- Peel survival rate

**Links**  
- Upstream: [C-13](#c-13), [A-09](#a-09)  
- Downstream: [D-21](#d-21), [D-23](#d-23)

---

<a id="d-14"></a>
### D-14 — HQ Recognition OS (Split-Squat Junction Alert)

**Purpose (plain English)**  
HQ is a high-risk junction where backstep/turn-away resets are imminent. Recognition must be immediate so you suppress the exit before it happens.

**Trigger**  
- Opponent establishes split-squat / HQ engagement

**Reads**  
- Which reset exit is coming:
  - `EXIT: BACKSTEP`
  - `EXIT: TURN-AWAY`
  - `EXIT: FLEE`

**Outputs**  
- Early suppression priority (stop exit first, then progress)

**Run it (fast)**  
1) Recognize HQ instantly.  
2) Identify the primary exit attempt.  
3) Suppress that exit before attacking ([D-23](#d-23), then [D-24](#d-24)/[D-25](#d-25)).

**DO / DON’T**  
- **DO:** Stop the reset first.  
- **DON’T:** Chase offense while exit is live.

**Failure signatures**  
- You notice HQ after the backstep already created distance.  
- You attack and opponent cleanly resets.

**Metrics**  
- HQ recognition latency  
- Backstep reset rate from HQ

**Links**  
- Downstream: [D-24](#d-24), [D-23](#d-23), [D-21](#d-21)

---

<a id="d-15"></a>
### D-15 — DLR Outside-Control OS (Outside Track = No Free Step-Away)

**Purpose (plain English)**  
DLR functions only if you control the outside track so they can’t step away and reset. Outside control + redundancy forces predictable steps and creates conversion windows.

**Trigger**  
- DLR engaged or attempted  
- Opponent trying to peel and step-away to reset

**Reads**  
- Can they step-away cleanly?  
- Can you survive peel #1 and maintain outside control?

**Outputs**  
- Step map forced + predictable reactions → conversion windows

**Run it (fast)**  
1) Establish outside control that restricts step-away.  
2) Install second connection immediately ([D-16](#d-16)).  
3) Force step map ([B-08](#b-08)).  
4) Convert on reaction windows ([D-01](#d-01)).

**DO / DON’T**  
- **DO:** Treat “no free step-away” as the KPI for DLR.  
- **DON’T:** Assume DLR is on just because a hook exists.

**Failure signatures**  
- Opponent disengages for free; repeated resets.  
- First peel clears everything.

**Metrics**  
- Forced steps/posts per minute from DLR  
- Peel survival rate (beat #1)  
- Step-away resets allowed per round

**Links**  
- Upstream: [A-10](#a-10), [B-16](#b-16)  
- Downstream: [D-23](#d-23), [D-22](#d-22)

<a id="d-16"></a>
### D-16 — Second Connection Rule OS (Redundancy Within 1–2 Beats)

**Purpose (plain English)**  
First connection is temporary. Second connection makes it real. This rule prevents one-peel resets and stabilizes every entry/platform.

**Trigger**  
- The moment you establish any meaningful first connection (leg handle, platform, clamp)  
- Any time you catch yourself progressing from single-point contact

**Reads**  
- Connection count (1 vs 2+)  
- Opponent’s peel/strip readiness (hands active, retreat cues)

**Outputs**  
- A redundant control structure that survives defense beat #1 and #2

**Run it (fast)**  
1) Gain first connection.  
2) Install second connection within 1–2 beats.  
3) Only then progress to consolidation/finish.

**DO / DON’T**  
- **DO:** Treat “second connection” as mandatory before ambition.  
- **DON’T:** Attack from a single-point handle.

**Failure signatures**  
- First peel clears everything.  
- You repeatedly “get there” but can’t keep it.

**Metrics**  
- Time to second connection after first contact  
- First-peel survival rate

**Links**  
- Upstream: [B-16](#b-16), [B-05](#b-05)  
- Downstream: [D-17](#d-17), [D-23](#d-23)

---

<a id="d-17"></a>
### D-17 — Entry-to-Consolidation Bridge OS (No “Access Only”)

**Purpose (plain English)**  
Entries are worthless if they don’t become a stable structure. This OS forces every entry to immediately convert into consolidation that denies retract/turn-out/reset.

**Trigger**  
- Any successful entry contact (single/double/platform leg access)  
- Any time you “touch legs” but feel unstable

**Reads**  
- Can you deny immediate retract/turn-out?  
- Did you install second connection? ([D-16](#d-16))

**Outputs**  
- Installed consolidation structure (cross-catch / hip-pin / knee-line containment)

**Run it (fast)**  
1) Entry contact achieved.  
2) Install second connection ([D-16](#d-16)).  
3) Install consolidation structure ([D-18](#d-18), [D-19](#d-19)).  
4) Monitor knee line and suppress escape ([D-20](#d-20)).

**DO / DON’T**  
- **DO:** Consolidate before chasing finishes.  
- **DON’T:** Scramble in “access mode” and donate separation.

**Failure signatures**  
- Opponent retracts and resets cleanly.  
- You lose control on first turn-out.

**Metrics**  
- Entry→consolidation time  
- % entries surviving first clear attempt

**Links**  
- Downstream: [D-18](#d-18), [D-19](#d-19), [D-20](#d-20), [D-23](#d-23)

---

<a id="d-18"></a>
### D-18 — Cross-Catch Consolidation OS (Contain Retract + Rotation)

**Purpose (plain English)**  
Convert leg access into containment that prevents clean retraction and limits rotational exits. This is the first “make it stick” consolidation layer.

**Trigger**  
- After leg access is achieved  
- Opponent attempts to retract leg or pivot out

**Reads**  
- Retract attempts (foot/knee line pulling free)  
- Rotation attempts (hip turning to exit)

**Outputs**  
- Stable containment that denies clean retract/turn-out long enough to progress

**Run it (fast)**  
1) Establish cross-catch structure.  
2) Test: can they retract cleanly? can they rotate freely?  
3) If rotation is still live, add hip-pin layer ([D-19](#d-19)).  
4) Maintain knee line ([D-20](#d-20)).

**DO / DON’T**  
- **DO:** Test containment immediately (don’t assume).  
- **DON’T:** Chase progress while retract/rotation is still free.

**Failure signatures**  
- Leg retracts cleanly on first defense.  
- Opponent pivots out while you chase.

**Metrics**  
- Hold time under resistance  
- Clean retract escapes allowed (%)

**Links**  
- Next: [D-19](#d-19), [D-20](#d-20)

---

<a id="d-19"></a>
### D-19 — Hip-Pin Consolidation OS (Suppress Rotation First)

**Purpose (plain English)**  
Rotational freedom is the main escape engine. Hip-pin suppresses rotation so your consolidation doesn’t evaporate into turn-aways/backsteps.

**Trigger**  
- Opponent begins turning hips to escape  
- After cross-catch when rotation pressure appears

**Reads**  
- Rotation direction (which way they are turning to unwind)  
- Is rotation still free after your first containment attempt?

**Outputs**  
- Rotation suppressed; stabilization achieved; exit paths narrowed

**Run it (fast)**  
1) Identify rotation direction.  
2) Apply hip-pin/suppression that blocks that rotation.  
3) Re-test: is rotation still available? If yes, re-tighten before progressing.

**DO / DON’T**  
- **DO:** Stabilize rotation before pursuing finish outcomes.  
- **DON’T:** Trade stabilization for speed (you’ll get reset).

**Failure signatures**  
- You chase progress and opponent turn-aways/backsteps out.  
- You “feel close” but can’t keep them contained.

**Metrics**  
- Rotation escape frequency after consolidation begins  
- Time to suppress rotation after attempt starts

**Links**  
- Next: [D-20](#d-20), [D-23](#d-23)

---

<a id="d-20"></a>
### D-20 — Knee-Line Containment OS (Don’t Let Base Rebuild)

**Purpose (plain English)**  
If the knee line escapes, the opponent rebuilds base and your entire entry loses value. Knee-line control is the “keep the base broken” layer.

**Trigger**  
- Opponent tries to pull knees free, widen base, or stand/retract after your entry  
- Any time you feel knee line slipping

**Reads**  
- Knee line status: captured vs slipping  
- Opponent widening/retracting behavior

**Outputs**  
- Knee line retained; base recovery denied; continuation of consolidation

**Run it (fast)**  
1) Monitor knee line continuously (not occasionally).  
2) If it slips, recapture immediately (before chasing progress).  
3) Rebuild redundancy if needed and continue consolidation.

**DO / DON’T**  
- **DO:** Treat knee-line slippage as highest priority.  
- **DON’T:** Ignore knee line while pursuing “finish” actions.

**Failure signatures**  
- Knees slip free → opponent stands/backs out → reset.  
- You had control but lost it during ambition.

**Metrics**  
- Knee-line recapture success rate  
- Resets occurring after knee-line slip events

**Links**  
- Downstream: [D-21](#d-21), [D-23](#d-23), [D-27](#d-27)

<a id="d-21"></a>
### D-21 — Platform-to-Hub Routing OS (Choose Stabilization by Exit)

**Purpose (plain English)**  
You don’t pick stabilization by preference; you pick it to suppress the opponent’s current escape. Routing is “exit-first decision making.”

**Trigger**  
- After platform is established and opponent starts escaping  
- After consolidation begins and you feel them trying to reset distance

**Reads**  
- Primary exit attempt (which one restores distance fastest):
  - `EXIT: BACKSTEP`
  - `EXIT: FLEE`
  - `EXIT: TURN-AWAY`
  - `EXIT: PEEL/STRIP`

**Outputs**  
- Correct routing choice + suppression priority (stop exit first)

**Run it (fast)**  
1) Identify primary exit attempt.  
2) Choose stabilization response that blocks that exit.  
3) Stabilize first; only then progress/finish.

**DO / DON’T**  
- **DO:** Stop the exit that restores distance fastest.  
- **DON’T:** Stabilize into a structure that allows their preferred reset.

**Failure signatures**  
- You “get control” but opponent resets anyway.  
- You stop a secondary motion and allow primary escape.

**Metrics**  
- Exit suppression rate after routing decision  
- Resets allowed after platform established (%)

**Links**  
- Downstream: [D-22](#d-22), [D-23](#d-23), [D-27](#d-27)

---

<a id="d-22"></a>
### D-22 — Exit-Based Hub Selection OS (Universal Reset Classifier)

**Purpose (plain English)**  
A general classifier that tags the opponent’s reset behavior so the correct follow/contain response is automatic.

**Trigger**  
- Any time opponent attempts to reset distance or strip control

**Reads**  
- `EXIT` classification:
  - FLEE (backing out/running away)
  - BACKSTEP (hip rotation + step around to disengage)
  - TURN-AWAY (turning hips away to unwind)
  - PEEL/STRIP (hand-fighting your connection off)

**Outputs**  
- Correct anti-exit response selection

**Run it (fast)**  
1) Classify the exit.  
2) Execute the matching follow/contain response.  
3) Rebuild connection + force new proof window.

**DO / DON’T**  
- **DO:** Follow immediately while maintaining attachment.  
- **DON’T:** Chase after you’ve already lost contact.

**Failure signatures**  
- Repeated clean resets.  
- Late follow with no connection.

**Metrics**  
- Time exit begins → reattachment  
- Resets allowed per round

**Links**  
- Downstream: [D-24](#d-24), [D-25](#d-25), [D-26](#d-26), [D-23](#d-23)

---

<a id="d-23"></a>
### D-23 — Anti-Exit Master OS (No Free Resets)

**Purpose (plain English)**  
Convert your control into a persistent loop. Every disengagement attempt is treated as a trigger to maintain at least one connection and reassert control.

**Trigger**  
- Any backstep/flee/turn-away/peel reset attempt  
- Any time opponent tries to return to long range

**Reads**  
- Which exit is occurring (use [D-22](#d-22))  
- Do you still have at least one connection? (must be yes)

**Outputs**  
- Attachment maintained through the reset attempt + immediate re-control loop restart

**Run it (fast)**  
1) Detect exit early.  
2) Follow immediately while keeping one connection.  
3) Rebuild second connection ([D-16](#d-16)).  
4) Force new reaction/proof and convert ([B-03](#b-03), [D-01](#d-01)).

**DO / DON’T**  
- **DO:** Preserve attachment; attachment is the follow engine.  
- **DON’T:** Accept resets as “normal.” They are failures unless chosen.

**Failure signatures**  
- Opponent repeatedly returns to long range.  
- You follow late and arrive after they are stable.

**Metrics**  
- Reset attempts denied (%)  
- Reattachment time after exit begins

**Links**  
- Downstream: [D-24](#d-24), [D-25](#d-25), [D-26](#d-26)

---

<a id="d-24"></a>
### D-24 — Backstep Follow OS (Track the Rotation Early)

**Purpose (plain English)**  
Deny backstep reset by following the hip rotation early and reattaching before they square up at distance.

**Trigger**  
- `EXIT: BACKSTEP` detected

**Reads**  
- Hip rotation cue (the moment it begins)  
- Which connection point will survive the turn?

**Outputs**  
- Backstep contained; reattachment preserved

**Run it (fast)**  
1) Recognize rotation early.  
2) Follow the rotation (don’t chase where they were).  
3) Reattach and rebuild redundancy before they square up.

**DO / DON’T**  
- **DO:** Follow on the first rotation cue.  
- **DON’T:** Follow after distance is restored (too late).

**Failure signatures**  
- Full reset created by backstep.  
- You chase after losing attachment.

**Metrics**  
- Backstep resets allowed per round  
- Rotation cue → reattachment time

**Links**  
- Part of: [D-23](#d-23)

---

<a id="d-25"></a>
### D-25 — Flee Follow OS (No Free Retreat)

**Purpose (plain English)**  
When the opponent retreats to reset stance, you maintain attachment and occupy space so they can’t restart stable.

**Trigger**  
- `EXIT: FLEE` detected (backing away / disengaging)

**Reads**  
- Retreat direction and speed  
- Can you keep at least one connection during retreat?

**Outputs**  
- Continuous attachment through retreat + forced re-engagement

**Run it (fast)**  
1) Treat retreat as immediate trigger.  
2) Follow while maintaining at least one connection.  
3) Rebuild redundancy and force step map again ([B-08](#b-08)).

**DO / DON’T**  
- **DO:** Maintain attachment; don’t “run after them.”  
- **DON’T:** Let them reset stance cleanly.

**Failure signatures**  
- Repeated long-range resets.  
- You chase without attachment and arrive late.

**Metrics**  
- Retreat resets allowed per round  
- Retreat cue → reattachment time

**Links**  
- Part of: [D-23](#d-23)

---

<a id="d-26"></a>
### D-26 — Peel/Strip Counter-Loop OS (Strip → Replace → Redundancy)

**Purpose (plain English)**  
Strips are predictable beats. This loop makes strip attempts convert into your reattachment tempo rather than a reset.

**Trigger**  
- `EXIT: PEEL/STRIP` detected  
- Any time opponent attacks your connection points

**Reads**  
- What got stripped + what remains connected

**Outputs**  
- Connection retained or immediately restored; redundancy rebuilt; control loop resumes

**Run it (fast)**  
1) Expect peel #1.  
2) Maintain one connection through peel if possible; otherwise replace immediately ([B-06](#b-06)).  
3) Rebuild second connection ([D-16](#d-16)).  
4) Resume forcing reactions and converting ([B-03](#b-03), [D-01](#d-01)).

**DO / DON’T**  
- **DO:** Replace instantly; don’t negotiate with the strip.  
- **DON’T:** Reattach once and stop—rebuild redundancy or you’ll be stripped again.

**Failure signatures**  
- First peel clears everything.  
- You reattach but get stripped immediately again.

**Metrics**  
- Strip → replacement time  
- Peel survival rate (beat #1)

**Links**  
- Part of: [D-23](#d-23)

---

<a id="d-27"></a>
### D-27 — Stabilize-Then-Finish Governance OS (Greed Control)

**Purpose (plain English)**  
Near-finish attempts that allow resets are net negative. If the primary exit is live, stabilize first; finish second.

**Trigger**  
- You’re close to an outcome but opponent still has a clean reset exit  
- You feel tempted to “go now” without suppression

**Reads**  
- Is the primary exit still live? (yes/no)  
- Which exit is it? ([D-22](#d-22))

**Outputs**  
- Either stabilization step (suppress exit) or permission to finish

**Run it (fast)**  
1) Identify primary exit.  
2) If exit live → stabilize to suppress ([D-21](#d-21), [D-23](#d-23)).  
3) Once suppressed → finish attempt.

**DO / DON’T**  
- **DO:** Governance beats greed.  
- **DON’T:** Trade stability for “almost.”

**Failure signatures**  
- You chase finish and opponent resets.  
- You win a moment and lose the exchange.

**Metrics**  
- Finish attempts ending in reset (%)  
- Time to suppress exit before finishing

___

Footer 
	•	Last updated: YYYY-MM-DD
	•	Change log:
	•	YYYY-MM-DD — Initial full draft (Buckets A–D, Quick Router, Glossary)









