PATH: SYS/Guard/Open-Guard/entries_rdrl_part-1_base-break-platform.md

# Entries (RDLR) — Part 1: Base-Break Platform (Hands-to-Mat → Heel Exposure)

## 1. Purpose
Use **Reverse De La Riva (RDLR)** as a reliable platform to:
- **break base** by forcing **hands to the mat**, and
- create a **locked leg configuration** (leg behind + foot in front) that yields **automatic heel exposure** and leads to strong finishing positions.

This is the “platform” layer: establish the wedge/containment structure and the base-break invariant before any advanced variations.

## 2. Inputs / Preconditions
- Opponent is standing and driving in, or pressing you flat (forward pressure present).
- You can establish the **RDLR hook** as they come forward.
- You can secure **calf control** (wrist deep; not fingers).
- You can create or accept a moment where opponent’s posture is compromised enough to put **hands to mat**.

## 3. Outputs / Success Criteria
- Opponent’s **hands touch the mat** (base-break achieved).
- You have the core lock:
  - **one leg behind** the opponent’s target leg,
  - **one foot wedging in front** (wedge + containment).
- You can rotate/turn inside and use a **knee-reap direction** to point their knee across your hip line.
- You pummel through to a position that gives **automatic heel exposure** (heel lands on/near top shoulder).
- You can immediately stabilize a finish line (belly-down/knee line control) and deny key exits (pull-away/backstep).

## 4. Core Model / Engine
**RDLR HOOK → CALF CONTROL → HANDS DOWN → KNEE ACROSS HIP (knee-reap) → FOOT PUMMEL THROUGH → AUTO HEEL EXPOSURE → STABILIZE**

Operational sequence (platform build):
1) Opponent drives forward → you install **RDLR hook**.
2) Secure **calf** with wrist depth (no fingers).
3) Force **hands to the mat** (base-break invariant).
4) Pull/steer so their knee faces **across your hip** (use the knee-reap direction; don’t try to throw your leg over a straight leg).
5) Post with second hand to prevent knees coming together.
6) Pummel your foot through and hook in front → heel is now trapped on top shoulder → **automatic heel exposure**.
7) Convert to belly-down/knee control finish line; govern pull-away/backstep.

## 5. Gates (override rules)

### 5.1 Hands-to-Mat Gate (base-break invariant)
If hands are not on the mat, your structure is not yet “locked” enough for reliable progression.
- **Default action:** prioritize base-break: pull + wedge + angle until hands post.

### 5.2 “No Straight-Leg Throw” Gate (mechanical constraint)
Trying to throw your leg over a straight leg fails.
- **Default action:** use the knee-reap direction first to bend/point their knee across your hip, then pummel.

### 5.3 Wrist-Depth Calf Grip Gate (control quality)
Fingers-in grip reduces control and invites slips.
- **Default action:** go in with the wrist; clamp calf.

### 5.4 Anti-Pull-Away Gate
If opponent tries to pull away, you must convert immediately to a locking posture.
- **Default action:** knee to floor + lock connection; keep heel exposure.

### 5.5 Anti-Backstep Gate (distance governance)
If opponent backsteps, you must control distance; if your knee points to ceiling you lose distance control.
- **Default action:** place foot at the **center line** (center stomach/chest line) to govern distance; then bring legs together, lock, and transition to inside-shoulder finishing alignment.

## 6. Top-6 Situations Playbook
1) **Opponent drives you flat**  
   → **Default:** RDLR hook + calf control; begin base-break plan.

2) **You have RDLR hook but opponent’s hands are free**  
   → **Default:** pull/angle until hands post (do not rush pummel).

3) **Opponent’s leg is straight and you want to pummel**  
   → **Default:** knee-reap to bend/point knee across hip first.

4) **You achieved hands-to-mat**  
   → **Default:** pummel through to front hook; take automatic heel exposure.

5) **Opponent tries to pull away**  
   → **Default:** knee to floor + lock; deny escape and finish line.

6) **Opponent backsteps**  
   → **Default:** foot to center line to govern distance; follow to inside shoulder and finish.

## 7. Opponent Reactions → Responses
- **Drives forward / presses flat:** install hook; clamp calf; base-break to hands down.
- **Tries to bring knees together:** post with second hand so knees can’t close; keep knee-reap direction.
- **Pulls away:** knee to floor + lock; keep heel trapped.
- **Backsteps:** foot to center line to govern distance; bring legs together; inside-shoulder finish alignment.
- **Handfights forward:** barrier effect increases when center-line foot is placed; use the time to lock/finish.

## 8. Failure Signatures → Fix
- **“I can’t pummel through.”** → you tried on a straight leg; enforce knee-reap first.
- **“My grip slips.”** → fingers-in; switch to wrist-depth calf grip.
- **“He backsteps and I lose him.”** → you didn’t govern distance; foot to center line immediately.
- **“He pulled away and escaped.”** → you didn’t drop knee/lock; convert to locking posture sooner.
- **“Hands never go to mat.”** → you skipped base-break; treat hands-down as the entry invariant.

## 9. Trigger Recognition Checklist
Proceed to pummel/finish line when 2+ cues are true:
- [ ] opponent’s hands are on the mat (or clearly posting)
- [ ] you have leg-behind + wedge-in-front containment
- [ ] opponent’s knee is pointed across your hip (knee-reap achieved)
- [ ] second hand is posted to prevent knees closing

## 10. Quality / Capture Checklist
- [ ] calf grip is wrist-deep and stable
- [ ] hands-to-mat base break is achieved
- [ ] knee-reap direction is set (no straight-leg pummel attempts)
- [ ] foot pummel creates front hook and heel lands on/near top shoulder (auto exposure)
- [ ] backstep distance governance is ready (center-line foot)
- [ ] pull-away lock is ready (knee-to-floor + lock)

## 11. Interfaces (routing rules)
- `governance_anti-backstep.md` — use when: opponent backsteps and you must govern distance and follow.
- `governance_anti-flee_the-mat.md` — use when: opponent’s primary defense is pull-away/disengage.
- `hub_criss-cross_inside-outside_backside-stability.md` — use when: you transition to the inside/outside compromise entanglement for stronger barriers + containment.
- `hub_double-50_multi-leg-control.md` — use when: you choose multi-leg containment to deny pull-away and backstep.
- `hub_50-50_turn-away-containment.md` — use when: classic containment is the required fallback.
- `hub_inside-senkaku_forward-barrier.md` — use when: your progression yields a forward-barrier inside position that stabilizes turn-in attacks.

## 12. Diagram
~~~
RDLR BASE-BREAK PLATFORM

[Opponent drives forward / presses flat]
               |
               v
        [RDLR hook + calf (wrist) grip]
               |
               v
     [Base-break: get HANDS to MAT]
               |
               v
 [Knee-reap -> point knee across hip]
  (no straight-leg throw attempts)
               |
               v
   [Post 2nd hand: deny knees closing]
               |
               v
   [Foot pummel through -> front hook]
               |
               v
 [Heel trapped on top shoulder = AUTO exposure]
               |
               +--> if pull-away: knee to floor + lock
               |
               +--> if backstep: foot to center line -> lock -> inside-shoulder finish
~~~

## 13. Drills and Games

### 13.1 Hands-to-Mat Invariant Game
- **Start:** opponent standing, driving in; you start with RDLR hook and calf grip.
- **Defender wins:** force hands-to-mat within 10s and pause 2s in locked wedge structure.
- **Passer wins:** keep hands free for 10s or disengage to two steps.
- **Rules:** no pummeling/finishing until hands touch mat.
- **Reset:** 2s pause or timer.
- **Rounds:** 10 reps each, switch.

### 13.2 Knee-Reap Before Pummel (constraint drill)
- **Start:** hands-to-mat achieved; opponent keeps leg straight as long as possible.
- **Defender wins:** achieve knee-reap direction (knee across hip) then pummel through to front hook (pause 2s).
- **Passer wins:** prevent knee-reap/pummel for 10s.
- **Rules:** any “throw leg over straight leg” attempt is rep loss.
- **Reset:** 2s pause or timer.
- **Rounds:** 8 reps each, switch.

### 13.3 Backstep Distance Governance
- **Start:** you have auto heel exposure; opponent’s only defense is backstep.
- **Defender wins:** place foot to center line and prevent clear escape for 5s.
- **Passer wins:** complete backstep escape within 5s.
- **Rules:** if your knee points to ceiling while backstep happens, rep loss (must govern distance).
- **Reset:** 5s hold or escape.
- **Rounds:** 8 reps each, switch.