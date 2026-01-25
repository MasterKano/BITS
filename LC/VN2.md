## VN2 — Top 20 Systems (Ranked by Significance) (Operational Density)

### 1) Context Laws Decision OS
**Trigger:** Any decision point in guard (before denial, entry, or during scramble).  
**Objective:** Select the correct action family using 3 filters: kneeling/standing/head height.  
**Rules:** Kneeling = shoulders/hips; Standing = heels/toes; Head = under/over → mode.  
**Failure signature:** Random technique choice; forcing low-% actions into wrong posture.  
**Metric:** Correct context calls per round; correct family selection rate.

---

### 2) Six-Element Passing Chain Model OS
**Trigger:** Any time you need to diagnose passer progress.  
**Objective:** Model passing as requirements chain: Distance→Grip→Angle→Level→Penetration→Pin.  
**Rules:** Break the active link early; later links are higher cost.  
**Failure signature:** Defending “pass names” instead of requirements; late defense default.  
**Metric:** Correct link ID rate; reduced time in penetration/pin.

---

### 3) Knowledge/Denial Micro-Cycle OS
**Trigger:** Opponent begins building any pass requirement.  
**Objective:** Identify→deny→re-center→re-attach→convert (repeatable retention unit).  
**Rules:** Denial is incomplete without re-centering and re-attachment.  
**Failure signature:** Win the moment, lose the next step; denial without conversion.  
**Metric:** Cycle completion rate; conversions during repair-step window.

---

### 4) Active-Link Identification OS
**Trigger:** Pressure increases or choices multiply.  
**Objective:** Declare the single dominant link being built now.  
**Rules:** If two links develop, deny the earlier one; reassess after each denial.  
**Failure signature:** Fighting grips while angle is being won (wrong problem).  
**Metric:** Correct first-link calls; % denials preventing next-link progression.

---

### 5) Early-Denial Triage OS
**Trigger:** Overwhelm or accelerated passing.  
**Objective:** Apply fixed priority: Distance, Grip, Angle, Level, then emergency Penetration/Pin.  
**Rules:** Bias to early denial; treat late chain as high-cost emergency states.  
**Failure signature:** Constant emergency defense; rapid fatigue; pin events.  
**Metric:** Early-to-late denial ratio; pin events per round.

---

### 6) Head Under/Head Over Mode Selection OS
**Trigger:** Choosing under/elevation vs come-up/rise options.  
**Objective:** Select correct mode from head height / hips-back posture.  
**Rules:** Head high → under-mode available; head low/hips back → up-mode or posture change first.  
**Failure signature:** Under-rotation into hips-back posture; separation/reset donated.  
**Metric:** Correct mode calls; reduction in failed under entries.

---

### 7) Standing Heels–Toes Law OS
**Trigger:** Opponent is standing.  
**Objective:** Read weight distribution to predict step options and entry validity.  
**Rules:** Even weight = low validity until you force step/post; heels vs toes informs commitment.  
**Failure signature:** Entering into stable base without proof.  
**Metric:** Step prediction accuracy; entries preceded by forced weight commitment.

---

### 8) Kneeling Shoulders–Hips Law OS
**Trigger:** Opponent is kneeling.  
**Objective:** Use shoulders/hips alignment to choose pressure responses and avoid bad rotations.  
**Rules:** Shoulders leading = pressure; hips/stacked = create proof first before committing.  
**Failure signature:** Forcing rotations into stable kneeling posture; losing connection.  
**Metric:** Correct read rate; proof-gated entries in kneeling context.

---

### 9) Dynamic Energy Read OS
**Trigger:** Any time opponent changes pressure direction (drive, withdraw, redirect).  
**Objective:** Predict next step/posture shift by reading commitment.  
**Rules:** Classify energy state; choose actions that exploit commitment instead of colliding with it.  
**Failure signature:** Moving into their strength; mis-timed actions.  
**Metric:** Read accuracy; % predicted steps/posture shifts.

---

### 10) Retention-First Priority OS
**Trigger:** Pass-chain construction begins.  
**Objective:** Enforce retention as the first skill: deny build before offense.  
**Rules:** Prefer early denial; after denial, convert to threat immediately (no neutral drift).  
**Failure signature:** Only responding at penetration/pin; offense attempted while losing guard.  
**Metric:** Time spent in late-chain states; early denial frequency.

---

### 11) Deny-and-Recenter OS
**Trigger:** After any successful denial action.  
**Objective:** Prevent “moment wins” from turning into next-step losses.  
**Rules:** Denial must be followed by re-centering alignment before advancing.  
**Failure signature:** You break a link, but angle/level returns instantly.  
**Metric:** % denials followed by re-centering within 1 beat.

---

### 12) Identify-Then-Act OS (No Blind Actions)
**Trigger:** When you feel urgency to “do something” under pressure.  
**Objective:** Force a diagnosis step before action selection.  
**Rules:** Identify context + active link first; then choose the smallest effective denial.  
**Failure signature:** Random actions; inconsistent outcomes.  
**Metric:** Correct diagnosis rate under time constraint.

---

### 13) Context × Chain Routing OS
**Trigger:** Any complex exchange where both posture and pass-link are changing.  
**Objective:** Combine context laws with active-link identification to route decisions cleanly.  
**Rules:** Context determines mode/family; chain determines what to deny first.  
**Failure signature:** Correct context but wrong denial priority (or vice versa).  
**Metric:** Decision coherence rate (correct context + correct active link).

---

### 14) Under-vs-Up Progression Mode OS
**Trigger:** When selecting whether to elevate/enter under vs come up/attack high.  
**Objective:** Maintain mode consistency based on head/hip posture signals.  
**Rules:** If posture denies under-mode, switch to up-mode until posture changes.  
**Failure signature:** Alternating modes randomly; donating separation.  
**Metric:** Mode stability (fewer mid-exchange mode flips without new cues).

---

### 15) Standing Commitment Detection OS
**Trigger:** Standing passer shifting weight or adjusting stance.  
**Objective:** Detect single-leg commitment as the basis for step map and proof.  
**Rules:** If weight is committed, force the next step; if not, manufacture commitment first.  
**Failure signature:** Attacking legs when both legs are “free.”  
**Metric:** % times you correctly identify committed leg before acting.

---

### 16) Kneeling Pressure Classification OS
**Trigger:** Kneeling passer begins pressure sequences.  
**Objective:** Classify whether pressure is upper-body (shoulders leading) or base-protected (hips stacked).  
**Rules:** Upper-body lead creates opportunities for posts/steps; stacked base requires proof creation first.  
**Failure signature:** Trying to “go under” stable stacked base.  
**Metric:** Correct classification rate; successful conversions after denial.

---

### 17) Link-Change Reassessment OS
**Trigger:** Immediately after you deny a link (or opponent changes tactic).  
**Objective:** Update the active-link diagnosis rather than continuing on the old problem.  
**Rules:** After every denial, re-identify the new active link (it will shift).  
**Failure signature:** Denying a link that is no longer active; drifting into late chain.  
**Metric:** Reassessment frequency; reduced “surprise penetration” events.

---

### 18) Late-Chain Emergency OS
**Trigger:** Penetration or pin threat appears (late chain).  
**Objective:** Treat late chain as emergency: stop progression, stabilize, and recover upstream.  
**Rules:** Resolve penetration/pin first, then fix upstream links so it doesn’t recur.  
**Failure signature:** Repeated late-chain emergencies without upstream correction.  
**Metric:** Pin escapes per round; recurrence interval of late-chain events.

---

### 19) Chain Integrity Rule OS (Don’t Let Links Combine)
**Trigger:** Opponent begins combining two links (e.g., grip+angle, angle+level).  
**Objective:** Break the earlier link to collapse the combination.  
**Rules:** Earlier link denial is cheaper and disrupts downstream links.  
**Failure signature:** You fight the later symptom; earlier cause remains.  
**Metric:** % times two-link attempts are stopped before penetration.

---

### 20) Repair-Step Window OS
**Trigger:** Opponent takes a stabilizing step after a denial.  
**Objective:** Convert during the repair step while base is re-stabilizing.  
**Rules:** Denial creates a short window; use it to re-attach, force proof, or initiate entry.  
**Failure signature:** Hesitation after denial; opponent repairs and restarts clean.  
**Metric:** Time denial→conversion; % conversions executed before stance stabilizes.
