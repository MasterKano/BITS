PATH: SYS/Guard/Open-Guard/open-guard_hub-handoffs.md

# Open Guard — Hub Handoffs (Single Router; No Duplication)

## Purpose
Single Open-Guard routing layer for leg-entanglement hubs. All hub mechanics live canonically in `SYS/leglocks/`.

## Canonical hubs used by Open Guard (go here for mechanics)
- `SYS/leglocks/control-hubs/hub_inside-senkaku_forward-barrier.md`
- `SYS/leglocks/control-hubs/hub_50-50_turn-away-containment.md`
- `SYS/leglocks/control-hubs/hub_double-50_multi-leg-control.md`
- `SYS/leglocks/control-hubs/hub_criss-cross_inside-outside_backside-stability.md`
- `SYS/leglocks/control-hubs/governance_hub-selection_rules.md`

## Handoff rules (Open Guard → Hub)

### 1) Inside Senkaku (forward barrier) — default first hub
**Use when**
- you land in inside entanglement off Open Guard entries (RDLR/HQ/DLR/X-bridge/closed-to-X)
- you can build a forward barrier and win knee line quickly

**Bail-out**
- knee line retracts repeatedly despite re-seating
- hip already cleared and opponent is already running (late)

### 2) 50/50 — turn-away containment
**Use when**
- turn-away/run is the dominant escape pattern
- you need a stable “stop-the-run” trade state before progressing

**Bail-out**
- knee line clears in one action repeatedly
- rotation still creates distance escape

### 3) Double 50 — containment upgrade
**Use when**
- 50/50 is present but clears/slips keep happening
- rotation/backstep keeps reopening exits

**Bail-out**
- upgrading causes loss of primary leg control
- contact breaks to distance (two steps)

### 4) Criss-cross — backside stability (pushing contest)
**Use when**
- exchange becomes legs-out push vs hands-peel
- backside stability is required before any progression

**Bail-out**
- relationship cannot be stabilized
- opponent clears hips to distance repeatedly

## Global exits (if hub engagement breaks)
- If opponent disengages to distance (two steps): route to distance re-capture (`entries_distance_*`).
- If you are being flattened: route to retention/framing layer first.

## Interfaces
- `SYS/Guard/Open-Guard/integration_vol-8_putting-it-together.md — use when: global Open Guard router.`
- `SYS/Meta/governance_anti-backstep.md — use when: backstep/rotation governs escape.`
- `SYS/Meta/governance_anti-flee_the-mat.md — use when: pull-away/disengage governs escape.`