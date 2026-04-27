# 🦍 HYBRID GORILLA 2.0

**A 36-week integrated training program for the runner who lifts.**

Built for: Steve Ricci · Age 43 · VO2max 52 · RHR 45 bpm · HRV ~70  
Goal: Sub-18:00 three-mile time trial by **December 31, 2026**  
Program start: **Monday, April 27, 2026**  
Current baseline: ~21:00 (7:00/mi · 8.57 mph)  
Total program: **249 days · 36 weeks · 5 phases**

---

## Table of Contents

1. [What This Is](#what-this-is)
2. [Version History](#version-history)
3. [Program Architecture](#program-architecture)
4. [Weekly Schedule](#weekly-schedule)
5. [Phase Structure](#phase-structure)
6. [Lift Sessions](#lift-sessions)
7. [Running Sessions](#running-sessions)
8. [Delt Finisher](#delt-finisher)
9. [Core / Abs Session](#core--abs-session)
10. [Conditioning Day](#conditioning-day)
11. [Travel Training](#travel-training)
12. [Nutrition & Supplement Protocol](#nutrition--supplement-protocol)
13. [Recovery Philosophy](#recovery-philosophy)
14. [Time Trial Checkpoints](#time-trial-checkpoints)
15. [App Features](#app-features)
16. [Equipment](#equipment)
17. [Foundational Sources & Philosophy](#foundational-sources--philosophy)
18. [Technical Notes](#technical-notes)
19. [Credits & Sources](#credits--sources)

---

## What This Is

Hybrid Gorilla 2.0 is a single-file, mobile-first progressive web app delivering a complete 36-week hybrid training program. Running and resistance training are fully integrated into one weekly schedule. The app lives in one self-contained HTML file with no dependencies, no backend, and no framework. All data — session completion, per-exercise weights, session notes, time trial results — is stored in the browser via localStorage.

The program bridges two worlds typically programmed in isolation: evidence-based hypertrophy methodology from the resistance training literature, and structured endurance running methodology from the Jack Daniels / VDOT framework. Neither discipline cannibalizes the other. Each is allocated volume and intensity based on its recovery cost relative to the shared recovery budget of a 43-year-old hybrid athlete.

The goal is simple and unambiguous: run three miles in under 18 minutes on December 31, 2026, from a current baseline of approximately 21 minutes. That is a 15% performance improvement over 36 weeks — achievable, not easy.

---

## Version History

### v1.0 (April 20, 2026)
Initial build. 36-week program, single HTML file, localStorage persistence. DB bench throughout, basic exercise selection, 4-tab UI (Today / Week / Plan / Paces). Program start April 20, race day December 26.

### v2.0 (April 27, 2026)
Full overhaul. All changes documented below under each relevant section. Key headline changes:

- **Lift program completely revised** — Olympic bar, landmine, bench progression, exercise substitutions throughout
- **Conditioning Day added** — replaces Upper B on Fridays from Phase 3 onward
- **Landmine Core Rotation** added program-wide as a rotational power anchor on Lower day and Conditioning Day
- **Nutrition tab added** — macro targets, timing protocol, full 7-compound supplement stack
- **Easy runs added to all lift days** — Mon/Wed/Fri each carry both a lift session and a 30–45 min easy run
- **Travel tracks restored** — Home / Travel Best / Travel Worst gym mode toggle with fully substituted exercise sets for all three lift sessions
- **Per-exercise weight logging** — number input field (lbs) on every exercise in every lift modal, stored per week/session/gym mode
- **Per-exercise done checkbox** — mark each movement as completed as prescribed, independent of session-level completion
- **Session notes** — free-text notes field per session per week, saves on every keystroke
- **Day preview from Plan and Week views** — tap any day or week to drill into the full session stack with working modals
- **Button fix** — replaced toString() action serialization with global action registry; all View Session buttons now work correctly
- **Program dates reset** — start April 27, race December 31, 249 total days

---

## Program Architecture

### Core Design Principles

**Recovery is the limiting variable.** The stimulus you cannot recover from is negative stimulus. Every programming decision — volume, intensity, session order, deload timing — flows from this principle. A 43-year-old running 6 days per week plus lifting 3 times plus weekly conditioning has a finite recovery budget. Spend it deliberately.

**Periodization is non-negotiable.** The program moves in phases. Volume and intensity relationships shift across phases in a deliberate pattern. Deloads are mandatory, not optional. Skipping them is the most common way a program breaks down.

**Neither goal cannibalizes the other.** The running and lifting are sequenced so that quality sessions in each discipline are not compromised by fatigue from the other. Lower body lifting is never within 48 hours of a quality run. The long run always has a clean recovery buffer.

**Progressive overload is the mechanism.** Every session references the previous session. More reps at the same weight, or same reps at more weight, is the definition of progress. Form is standardized in Phase 1 and never altered to chase numbers.

---

## Weekly Schedule

| Day | Phase 1–2 | Phase 3–5 |
|-----|-----------|-----------|
| **Monday** | Upper A + Easy Run | Upper A + Easy Run |
| **Tuesday** | Quality Run + Delt Finisher + Abs | Quality Run + Delt Finisher + Abs |
| **Wednesday** | Lower + Easy Run | Lower + Easy Run |
| **Thursday** | Quality Run + Delt Finisher + Abs | Quality Run + Delt Finisher + Abs |
| **Friday** | Upper B + Easy Run | **Conditioning Day** + Easy Run |
| **Saturday** | Long Run + Delt Finisher (opt) + Abs | Long Run + Delt Finisher (opt) + Abs |
| **Sunday** | Rest / Thunder 45 + Delt Finisher | Rest / Thunder 45 + Delt Finisher |

**Key structural notes:**
- Easy runs on Mon/Wed/Fri are 30–45 min at conversational pace — recovery and aerobic maintenance, not workouts
- Quality runs on Tue/Thu are the running stimulus — threshold, VO2max, and goal-pace work
- Saturday long run is aerobic base building — easy to moderate effort, never a race effort
- Sunday is genuine rest — Thunder 45 is optional conditioning, not mandatory
- Delt finisher runs on all non-lift days without exception: Tue, Thu, Sat, Sun
- Abs session runs daily — 10–12 min, can be done any time of day

---

## Phase Structure

### Overview

| Phase | Weeks | Dates | Name | Key Focus |
|-------|-------|-------|------|-----------|
| 1 | 1–8 | Apr 27 – Jun 21 | Foundation | Form, habits, DB bench, threshold intro, TT Wk 8 |
| 2 | 9–16 | Jun 22 – Aug 16 | Volume Bump | +20% delt/back/quad volume, goal-pace runs, TT Wk 16 |
| 3 | 17–24 | Aug 17 – Oct 11 | Transition | BB bench intro, Conditioning replaces Upper B, TT Wk 23 |
| 4 | 25–32 | Oct 12 – Dec 6 | Peak Running | Lifts maintenance, running peak volume, TT Wk 31 |
| 5 | 33–36 | Dec 7 – Dec 31 | Sharpen & Race | Taper, race-pace sharpening, Race Dec 31 |

### Deload Weeks

Mandatory deloads occur at Weeks 8, 16, 24, and 32. Protocol: sets halved, loads maintained, RIR raised to 3. These are not optional. Deload weeks are where adaptation is consolidated. The body does not get stronger during training — it gets stronger during recovery from training.

### RIR Progression

| Weeks | RIR Target |
|-------|-----------|
| 1–5 | RIR 2 → RIR 1 (progressive) |
| 6–7 | RIR 1–0 |
| 8 | DELOAD — RIR 3, sets halved |
| 9–15 | RIR 1–2 |
| 16 | DELOAD — RIR 3, sets halved |
| 17–23 | RIR 1 |
| 24 | DELOAD — RIR 3, sets halved |
| 25–31 | RIR 0–1 |
| 32 | DELOAD — RIR 3, sets halved |
| 33–36 | RIR 0–1 |

---

## Lift Sessions

### Flat Bench Press Progression

The bench press follows a deliberate 4-phase progression designed for joint and tendon health at 43. The barbell is not introduced until connective tissue is genuinely prepared for the stimulus.

| Phase | Implement | Sets × Reps | Focus |
|-------|-----------|-------------|-------|
| 1 (Wks 1–8) | DB flat bench | 3 × 8–12 | ROM standardization, 2–3 sec eccentric, full pec stretch |
| 2 (Wks 9–16) | DB flat bench | 3 × 6–10 | Load toward 75–90 lb DBs. Connective tissue conditioning. |
| 3 (Wks 17–24) | Olympic barbell | 3 × 8–12 | Intentional load drop. Bar path, wrist position, shoulder mechanics. |
| 4–5 (Wks 25–36) | Olympic barbell | 3 × 6–10 | Progressive overload resumes. Load builds to race day. |

**Rationale:** Heavy DB pressing through Phase 2 prepares the pec, anterior delt, and shoulder capsule for barbell loading. The higher rep range at Phase 3 barbell introduction is intentional — lighter absolute load means lower joint stress while the body adapts to the new implement. This adds approximately 8 weeks of connective tissue preparation compared to going straight to barbell in Phase 1.

---

### Upper A — Monday (All Phases)

*Chest · Back · Lateral Delt · Rear Delt · Arms · ~50 min*

| # | Exercise | Sets × Reps | Coaching Notes |
|---|----------|-------------|----------------|
| A1 | DB Bench (Ph 1–2) → BB Bench (Ph 3+) | 3 × 8–12 / 6–10 | Alternating with A2. See bench progression table above. |
| A2 | Weighted Pull-Up or Lat Pulldown | 3 × 6–10 | Alternating with A1. Add reps before adding weight. Full dead hang at bottom, chest to bar at top. |
| B1 | Landmine Press (single-arm, standing) | 2 × 10–12/arm | Alternating with B2. Stand perpendicular to landmine. Press at shoulder-friendly angle — hits upper chest, anterior delt, and rotational stability. Brace core throughout. |
| B2 | Landmine Row (single-arm) | 2 × 10–12/arm | Alternating with B1. Hinge at hip. Pull to hip crease. Natural arc deloads the wrist vs. DB row. Squeeze mid-back at peak. |
| C1 | Low Cable Lateral Raise | 4 × 12–15 | Low pulley. Slight forward lean. Lead with elbow, not hand. Full stretch at bottom. Phase 2+: 5 sets. |
| C2 | Cable Face Pull (rear delt) | 3 × 15–20 | High pulley. Pull to forehead. Externally rotate at peak. Squeeze rear delts — don't let traps take over. |
| D1 | Tricep Cable Pushdown (rope or bar) | 2 × 10–15 | Superset with D2. Elbows pinned to sides. Full extension at bottom. |
| D2 | DB Curl (standing or incline) | 2 × 10–12 | Superset with D1. Standing: supinate through the curl. Incline: greater long-head stretch. Alternate variation each session. |

**Maintenance (Phase 4–5):** A1, A2, B2, C1, C2 retained at 2 sets each. B1, D1, D2 dropped.

---

### Lower — Wednesday (All Phases)

*Posterior Chain · Nordic Curl · Single Leg · Calves · Rotational Core · ~50 min*

| # | Exercise | Sets × Reps | Coaching Notes |
|---|----------|-------------|----------------|
| A1 | Safety Bar Squat | 3 × 6–10 | Alternating with A2. SSB reduces anterior torque and spinal loading. Upright torso. Drive knees out. Sub: front squat or goblet squat. |
| A2 | Nordic Curl (modified eccentric) | 3 × 4–6 ecc | Alternating with A1. 5-count descent. Hands ready to catch. Ph 1–2: modified range. Ph 3+: fuller range. #1 evidence-based hamstring injury prevention for runners. |
| B1 | Romanian Deadlift (Olympic bar) | 3 × 6–10 | Alternating with B2. Hinge at the hip — not a squat. Bar in contact with legs throughout. Full stretch at bottom, squeeze glutes at lockout. |
| B2 | Roman Chair Back Extension | 3 × 10–15 | Alternating with B1. Hinge at hip — not spinal extension. Squeeze glutes hard at the top. BW first, then hold plate as it gets easy. |
| C1 | Rear-Foot-Elevated Split Squat (DB) | 2 × 8–10/leg | Front knee tracks over toes. Full depth — rear knee toward floor. Best running-specific strength movement in the program. Sub: walking lunge. |
| D1 | Standing Calf Raise (bar or DB) | 3 × 8–12 | Heavy. Full range — deep stretch at bottom, 1-sec hold at top. Non-negotiable for running economy and Achilles durability. |
| D2 | Cable Pull-Through or Hip Thrust | 2 × 10–15 | Glute-focused. Full lockout at top. Hip thrust: barbell across hips on bench. |
| E1 | Copenhagen Plank or Cable Adductor | 2 × 30s / 10–15 | Hip adductor stability. Critical for running stride integrity and groin health. |
| F1 | Landmine Core Rotation | 2–3 × 8–15/side | Power finisher. Rotate through hips, not just arms. Control the eccentric. Ph 1: 2×8–10/side light. Ph 2: 2×10–12/side moderate. Ph 3–5: 3×12–15/side power emphasis. |

**Maintenance (Phase 4–5):** A1, A2, B1, B2, D1, F1 retained at 2 sets. C1, D2, E1 dropped.

---

### Upper B — Friday (Phases 1–2 Only)

*Shoulders · Lateral Delt · Rear Delt · Back · Arms · ~50 min*
*Replaced by Conditioning Day in Phases 3–5.*

| # | Exercise | Sets × Reps | Coaching Notes |
|---|----------|-------------|----------------|
| A1 | Barbell OHP (Olympic bar, strict) | 3 × 6–10 | Alternating with A2. No leg drive. Full lockout at top. |
| A2 | Chin-Up or Supinated Cable Pulldown | 3 × 6–10 | Alternating with A1. Supinated grip increases bicep involvement. Full dead hang at bottom. |
| B1 | Weighted Dip (or DB Floor Press) | 2 × 8–12 | Alternating with B2. Upright = tricep emphasis. Slight forward lean = more chest. |
| B2 | Single-Arm Cable Row (half-kneeling) | 2 × 10–12/arm | Alternating with B1. Constant cable tension — different from Monday's landmine row. Emphasize full scapular retraction. |
| C1 | Lean-Away Cable Lateral Raise | 4 × 12–15 | Brace fixed object, lean away from cable. Greater loaded stretch than Monday's low-cable. Phase 2+: 5 sets. |
| C2 | Rear Delt Cable Fly (high pulley) | 3 × 15–20 | Slight forward hinge. Full arc to sides. Squeeze rear delts at peak. |
| D1 | DB Curl (preacher or standing) | 2 × 10–12 | Superset with D2. Alternate from Monday's variation. |
| D2 | Overhead DB Tricep Extension | 2 × 10–12 | Superset with D1. Full overhead stretch. Control the descent. |

---

### Delt Priority — Weekly Volume Accounting

| Source | Phase 1–2 Lateral Sets | Phase 3–5 Lateral Sets |
|--------|----------------------|----------------------|
| Upper A — Low Cable Lateral | 4–5 | 3 (maintenance) |
| Upper B — Lean-Away Cable Lateral | 4–5 | — (dropped) |
| Delt Finisher (4 non-lift days) | 2–3 × 4 = 8–12 | 3 × 4 = 12 |
| **Total lateral/week** | **~16–22 sets** | **~15 sets** |

Rear delt volume follows a similar pattern. Angle variation across Upper A (low cable), Upper B (lean-away cable), and the daily finisher ensures comprehensive lateral head stimulation.

---

### Nordic Curl Progression

Programmed Lower day A2 all 36 weeks, paired with safety bar squats. The strongest evidence base of any exercise for hamstring injury prevention in runners.

- **Phase 1–2:** Modified Nordic. Shins near-vertical. 5-count eccentric. Hands positioned to catch.
- **Phase 3+:** Fuller range as eccentric strength and tendon tolerance develop. Target is eventually a full straight-body descent from kneeling to floor.

---

## Running Sessions

### VDOT Framework

VO2max 52 → VDOT ~53 → predicted 5K ~18:15. The gap between current 21:00 and the ceiling is specific endurance, running economy, and neuromuscular tolerance of goal pace — all trainable.

**Goal pace:** 10.0 mph (6:00/mi). Sub-18:00 requires sustaining this for 18 minutes.

### Training Zones (Peloton Tread)

| Zone | Description | mph | min/mi | Purpose |
|------|-------------|-----|--------|---------|
| Easy (E) | Conversational · nasal breathing | 7.7–8.4 | 7:09–7:47 | Base, recovery, lift-day runs |
| Threshold (T) | Comfortably hard · ~1hr race effort | 9.0–9.5 | 6:19–6:40 | Lactate threshold elevation |
| Interval (I) | 5K race effort · VO2max | 9.5–10.5 | 5:43–6:19 | Raise aerobic ceiling |
| Repetition (R) | Short · fast · full recovery | 10.5–11.5 | 5:13–5:43 | Economy · neuromuscular sharpness |
| Goal Pace | Race target | 10.0 | 6:00 | Race-specific tolerance |

### Quality Runs (Tuesday + Thursday)

| Phase | Tuesday | Thursday |
|-------|---------|---------|
| 1 | 10 min E → 4×5 min @ T (9.0–9.5) w/ 90s rest → 10 min E | 10 min E → 5×3 min @ I (9.5–10.5) w/ 3 min jog → 10 min E |
| 2 | 10 min E → 5×5 min @ T w/ 90s rest → 10 min E | 10 min E → 6×2 min @ 10.0 mph w/ 2 min jog → 10 min E |
| 3 | 10 min E → 4×8 min @ T w/ 2 min rest → 10 min E | 10 min E → 8×1 min @ I w/ 2 min rest → tempo finish |
| 4 | Lactate threshold continuous 20–25 min | 10×1 min @ 10.0+ mph w/ 1:30 rest → 10 min E |
| 5 | 3×5 min @ T w/ 2 min rest (taper) | 6×1 min @ goal pace w/ 2 min rest (taper) |

### Long Runs (Saturday)

| Phase | Prescription | Duration |
|-------|-------------|---------|
| 1 | Easy pace · finish with 4×20s strides | 50–65 min |
| 2 | First 45 min easy → final 15 min progress to T pace | 60–75 min |
| 3 | Middle 30 min at 8.5–9.0 mph · easy bookends | 65–80 min |
| 4 | Peak volume · easy-to-moderate · 20 min at 8.5 mph | 70–90 min |
| 5 | Taper easy 30–40 min (Wks 33–35) · Race Dec 31 (Wk 36) | 30–40 min / Race |

### Easy Runs (Monday, Wednesday, Friday)

30–45 min · 7.7–8.4 mph · conversational pace. These are recovery runs, not workouts. Nasal breathing preferred. If they feel hard, you're running them too fast.

---

## Delt Finisher

Performed on all non-lift days: Tuesday, Thursday, Sunday, and optionally Saturday. Do not add to lift sessions.

### Phase 1–2 (~10 min)

| # | Exercise | Sets × Reps | Notes |
|---|----------|-------------|-------|
| 1 | Low Cable Lateral Raise | 2 × 15–20 | Light load, high quality. Lead with elbow. Full stretch at bottom. |
| 2 | Face Pull or Rear Delt Cable Fly | 2 × 15–20 | Squeeze rear delts at peak. Band or DB if no cable. |
| 3 | DB Shrug | 2 × 12–15 | Full depression at bottom. Drive straight up. 1-sec hold at top. No rolling. |

### Phase 3–5 (~12 min)

| # | Exercise | Sets × Reps | Notes |
|---|----------|-------------|-------|
| 1 | Low Cable Lateral Raise | 3 × 15–20 | Lead with elbow. Full stretch at bottom. |
| 2 | Rear Delt Cable Fly or Face Pull | 3 × 15–20 | Squeeze hard at peak. Don't let traps take over. |
| 3 | DB Shrug | 3 × 12–15 | Full depression to full elevation. 1-sec hold. Go heavy. |
| 4 | Band Pull-Apart | 2 × 20–25 | Arms straight. Pull to chest width. Shoulders down. |

---

## Core / Abs Session

Daily — 10–12 minutes — any time of day. Three movement patterns: flexion, anti-extension, rotational power (via landmine rotation on Lower day). Ab vacuums performed opportunistically throughout the day.

| # | Exercise | Sets × Reps | Pattern | Coaching Notes |
|---|----------|-------------|---------|----------------|
| 1 | Hanging Leg Raise | 3 × 8–12 | Flexion | Posterior pelvic tilt at top — pull the pelvis up, don't swing. Full control on descent. Sub: lying leg raise or captain's chair. |
| 2 | Cable Crunch (rope) | 3 × 10–15 | Flexion | Spinal flexion only — hips stay locked. Pull elbows toward knees, round the spine. Full stretch at top. |
| 3 | Ab Wheel Rollout or TRX Fallout | 2 × 8–12 | Anti-extension | Hollow body throughout — no lumbar arch. Arms fully extended at bottom. TRX fallout is an appropriate sub if ab wheel causes low-back discomfort. |
| 4 | RKC Plank | 2 × 20–30s | Irradiation | Not a rest. Full-body squeeze. Arms slightly forward of shoulders. Pull elbows toward feet and feet toward elbows simultaneously. |

---

## Conditioning Day

Replaces Upper B on Friday from Phase 3 onward. Anchored by a 10-rep-per-minute burpee EMOM — a format established during 7,500 burpees over 30 days in November 2025. The progression variable is duration (Phase 3→4) and vest load (Phase 4+), not reps per minute (locked at 10).

### Phase 3 (Weeks 17–24) — Power Foundation (~35 min)

| Block | Exercise | Prescription |
|-------|----------|-------------|
| Warm-Up | Easy jog or jump rope | 3 min |
| A | Burpee EMOM · bodyweight | 10 min · 10 reps/min · 100 total |
| B1 | Landmine Squat-to-Press (single-arm) | 3 × 8/arm · rest 90s |
| B2 | Swimmer's Curl (DB) | 3 × 12 · rest 60s |
| B3 | Landmine Core Rotation | 3 × 10/side · rest 60s |
| C | Trap Bar Farmer Hold | 3 × 45s · heavy · rest 90s |

### Phase 4 (Weeks 25–32) — Peak Metabolic Output (~40 min)

| Block | Exercise | Prescription |
|-------|----------|-------------|
| Warm-Up | Easy jog or jump rope | 3 min |
| A | Burpee EMOM · weighted vest | 15 min · 10 reps/min · 150 total · vest 15–20 lbs, add load across phase weeks |
| B — Circuit × 3 rounds | Landmine Squat-to-Press | 3 × 10/arm · 45s rest between rounds |
| | Swimmer's Curl (DB) | 3 × 15 · 45s rest |
| | Landmine Core Rotation | 3 × 12/side · 45s rest |
| C | Trap Bar Farmer Hold | 4 × 45s · heavier than Ph3 · rest 75s |

### Phase 5 (Weeks 33–36) — Sharpen (~32 min)

| Block | Exercise | Prescription |
|-------|----------|-------------|
| Warm-Up | Easy jog or jump rope | 2 min |
| A | Burpee EMOM · weighted vest | 10 min · 10 reps/min · 100 total · same vest as Phase 4 peak |
| B1 | Landmine Squat-to-Press | 2 × 8/arm · rest 90s |
| B2 | Swimmer's Curl (DB) | 2 × 12 · rest 60s |
| B3 | Landmine Core Rotation | 2 × 10/side · rest 60s |
| C | Trap Bar Farmer Hold | 2 × 45s · moderate · rest 90s |

**Key notes:**
- 10 reps/min is locked — duration and vest are the only levers
- Phase 4: B-block runs as circuit (B1→B2→B3, 45s rest between rounds). Phases 3 and 5: straight sets, 90s rest
- Vest introduced Phase 4 only — Phase 3 cements the pattern first
- Trap bar holds are isometric — grip, core, and postural endurance; heavy enough that 45s is genuinely challenging
- Saturday long run is the next morning — keep vest load honest in Phase 4 peak weeks

---

## Travel Training

Two exercise tracks available via the gym mode toggle (Home / Travel Best / Travel Worst) appearing on lift days in Today view. Weight logs are stored independently per gym mode.

### Travel Best Case
*Cable stack + adjustable DBs to ~60 lbs*

Full program replication with like-for-like substitutions. DB bent-over row for pull-up, DB single-arm shoulder press for landmine press, DB single-arm row for landmine row. Lower day uses DB goblet squat, floor-based Nordic curl (anchor feet), DB Romanian deadlift, Superman hold, and DB rotational chop. Upper B uses DB overhead press, towel row, DB floor press.

### Travel Worst Case
*Fixed DBs max ~30 lbs + treadmill only*

Compensated programming. Unilateral movements, tempo manipulation (2–3 sec eccentric), and higher rep ranges (12–20) replace heavy loading. Archer push-up for landmine press. Doorframe/towel row for pull movements. Prone Y-raise for rear delt. Bulgarian split squat for safety bar squat. Single-leg RDL for barbell RDL. All lateral delt work preserved via door frame lean-away technique.

---

## Nutrition & Supplement Protocol

### Athlete Profile

| Metric | Value |
|--------|-------|
| Age | 43 |
| Height | 6'0" |
| Bodyweight | 215 lbs |
| Body fat | ~13–16% (~14.5% midpoint) |
| Lean mass | ~184 lbs |
| TDEE | ~3,350 cal (Katch-McArdle BMR × 1.6 activity multiplier) |
| Target deficit | ~400 cal/day |
| Target fat loss | 0.5–0.75 lbs/week |

A 400-calorie deficit is the ceiling for this training volume at this age. Deeper deficits compromise running performance, increase injury risk, impair recovery, and sacrifice lean mass. The goal is simultaneous fat loss and performance improvement — achievable at appropriate deficit depth.

### Daily Macro Targets

| | Training Days (6×) | Rest Day (1×, Sun) |
|--|--|--|
| **Calories** | **3,000** | **2,600** |
| **Protein** | **220g (29%)** | **220g (34%)** |
| **Carbs** | **325g (43%)** | **215g (33%)** |
| **Fat** | **90g (27%)** | **95g (33%)** |

Weekly average: ~2,943 cal/day

**Protein** stays identical both days — muscle retention in a deficit requires consistent daily protein, not cycling. **Carbs** drop sharply on rest day — glycogen demand is minimal without training. **Fat** floor at ~90g (0.42g/lb BW) protects testosterone and hormonal function at 43. Do not go below this floor regardless of deficit depth.

### Fasted Training Context

All weekday training begins at 4:30am. Eating 1–2 hours before training would require a meal at 2–3am — not practical. All weekday sessions are trained fully fasted. Weekend sessions (Saturday long run, Sunday optional) start at 6:30–7:00am, which provides an optional small pre-workout snack window at ~6:00am if desired.

### Macro Timing

| Window | Focus | Targets |
|--------|-------|---------|
| Weekdays — pre-workout (4:00am) | Supplements only — no food | Fasted training. Supps taken on empty stomach. See protocol below. |
| Weekdays — post-workout / break fast (5:30–6:00am) | Protein + carb — priority #1 | 50g protein + 60–80g carbs. Most important meal of the day. Break the fast immediately after finishing. |
| Weekends — optional pre-workout snack (~6:00am) | Small, carb-forward | 30–40g carbs · 20g protein · minimal fat. Optional only — fasted is fine too. |
| Remaining meals — 2–3 across day | Distribute remaining macros | ~170g protein remaining after break-fast. Front-load carbs at lunch, taper toward evening. Keep fat low around training, distribute freely at later meals. |

### Supplement Protocol — 7 Compounds (Fasted-Adjusted)

#### Pre-Workout — ~4:00am weekdays / ~6:00am weekends (fasted)

| Supplement | Dose | Rationale |
|-----------|------|-----------|
| L-Citrulline | 6g pure or 8g malate 2:1 | Works well fasted — no food interference. Blood flow, endurance output, reduced soreness. Take 30–45 min before training. |
| L-Leucine | 3g | Most important fasted supplement in the stack. No dietary amino acids in the system pre-training — this is the only MPS trigger before the session. Non-negotiable for muscle retention in a fasted deficit athlete. |
| Beta-Alanine | 1.6g (dose 1 of 2) | Fine fasted. May feel more pronounced tingling on an empty stomach — normal and harmless. |
| Betaine Anhydrous (TMG) | 1.25g (dose 1 of 2) | Fine fasted. Take alongside the other pre-workout supplements. |

#### Post-Workout / Break Fast — within 30 min of finishing

| Supplement | Dose | Rationale |
|-----------|------|-----------|
| Protein | 50g | Priority #1. Training fasted means the body has been in a catabolic state through the session. Hit 50g protein immediately post-workout. Real food strongly preferred; powder if a full meal is not possible. |
| Creatine Monohydrate | 5g | Moved to post-workout for convenience — no morning meal precedes training. Take with break-fast meal. Timing does not affect efficacy; consistency does. |
| L-Carnitine L-Tartrate | 2g | Take with carbs from break-fast meal — insulin improves absorption significantly. Reduces muscle damage, supports fat oxidation. Pair with the carb portion of the first meal. |
| Beta-Alanine | 1.6g (dose 2 of 2) | Second daily dose. Take with break-fast meal. |
| Betaine Anhydrous (TMG) | 1.25g (dose 2 of 2) | Second daily dose. Pair with break-fast meal. |

#### Daily Schedule Summary

| Time | Supplements |
|------|------------|
| Pre-workout — 4:00am weekdays / 6:00am weekends | L-Citrulline 6g · L-Leucine 3g · Beta-Alanine 1.6g · Betaine 1.25g |
| Post-workout / break fast — ~5:30am weekdays / ~8:00am weekends | Protein 50g · Creatine 5g · L-Carnitine L-Tartrate 2g · Beta-Alanine 1.6g · Betaine 1.25g |
| Remaining meals | Distribute remaining macros across 2–3 meals |

*Evidence-based recommendations from published research and hybrid athlete protocols. Not personalized medical nutrition advice. Consult a physician or registered dietitian before beginning any new supplement regimen, particularly if on medication or managing health conditions.*

---

## Recovery Philosophy

### Non-Negotiables

- **Sleep: 7–8 hours per night.** The single highest-leverage recovery intervention. No supplement, nutrition strategy, or training modification compensates for chronic sleep restriction.
- **No lower body lifting within 48 hours before Thursday's VO2 session.** Lower day is Wednesday. The 48-hour window into Thursday's quality run is protected.
- **No lower body lifting the day before Saturday's long run.** Conditioning Day (Friday) is cardiovascular-dominant and does not compromise Saturday's long run.

### Nutrition Rules

- Deload weeks: maintenance or slight surplus — recovery is impaired by aggressive deficits during deloads
- Protein: 1.0–1.1g/lb every day regardless of training or rest status
- Carbohydrates: primary running fuel — not restricted on training days
- Fat: minimum 0.4g/lb every day for hormonal health

### Autoregulation — Bad Day Protocol

If 2+ of the following are true: poor recovery, bad sleep, elevated stress, missed meals, joint pain — apply the protocol:
- Lift sessions: 1 set per exercise at RIR 2–3, 12–15 reps. Complete the session, don't skip it.
- Quality runs: downgrade to easy fartlek — run easy with brief 30-second accelerations
- Log in session notes that the bad day protocol was applied

One bad day does not compromise a 36-week program. Skipping sessions does.

### Deloads

Weeks 8, 16, 24, 32. Sets halved, loads maintained, RIR 3. Non-optional. The body adapts during recovery from training, not during the training itself. Deloads are when the program pays dividends.

---

## Time Trial Checkpoints

Performed on the Saturday of the indicated week. Warm-up: 10 min easy. Test: 3.00 miles at maximal sustainable effort. Cool-down: 5–10 min easy. Results logged in the Paces tab.

| Week | Date | Target Time | Target Pace |
|------|------|-------------|------------|
| 0 | Apr 27, 2026 | ~21:00 (baseline) | 7:00/mi · 8.57 mph |
| 8 | Jun 20, 2026 | 20:00–20:30 | 6:47–6:50/mi |
| 16 | Aug 15, 2026 | 18:45–19:15 | 6:15–6:25/mi |
| 23 | Oct 3, 2026 | 18:30 | 6:10/mi |
| 31 | Nov 28, 2026 | 18:10–18:25 | 6:03–6:08/mi |
| **36** | **Dec 31, 2026** | **Sub 18:00** | **6:00/mi · 10.0 mph** |

---

## App Features

### Navigation

Five tabs: **Today / Week / Plan / Paces / Nutrition**

### Today View

Primary daily interface. Displays the complete session stack in order for the current day — lift session, easy run (lift days), quality/long run (run days), delt finisher, abs. Each session is a card with a colored left border: red = lift, blue = quality run, green = easy/long run, yellow = daily sessions, purple = conditioning.

On lift days, a gym mode toggle appears: **Home / Travel Best / Travel Worst**. Switching modes updates all session cards and modal content immediately.

Each session card contains: type label, title, meta description, "View Session →" button (opens full exercise modal), and a "Mark complete" checkbox that persists to localStorage.

Header displays: phase badge, week counter, day counter, race countdown in days, and a progress bar spanning all 249 program days.

### Week View

7-day layout with ← Prev / Next → navigation across all 36 weeks. Each day card shows day name, date, session title, and subtitle. Current day highlighted in red.

**Tap any day card** to open a full day preview modal showing every session for that day with working "View Session →" buttons. Tap the backdrop to dismiss.

### Plan View

All 5 phases as collapsible accordion cards. Current phase auto-expanded. Each phase shows its name, date range, and a training focus description. Each week within the phase shows its start date, any benchmark notes (time trials, deloads), and the RIR target.

**Tap any week row** (indicated by › chevron) to navigate directly to that week in the Week view. The Week tab activates automatically.

### Paces View

Training zone reference table in Peloton mph and min/mile, calibrated to the Peloton Tread. Includes Easy, Threshold, Interval, Repetition, and Goal Pace zones with current and target ranges.

Time trial log with editable input fields for all 6 checkpoints. Results persist in localStorage.

### Nutrition View

Full nutrition and supplement reference:
- Athlete profile (bodyweight, BF%, TDEE, deficit, target fat loss rate)
- Side-by-side macro targets: Training Days (6×) and Rest Day (1×)
- Macro timing protocol with specific gram targets per window
- Full 7-compound supplement protocol in three color-coded timing blocks: Morning (yellow), Pre-workout (blue), Post-workout (green)
- Each supplement entry includes name, exact dose, and mechanistic rationale

### Session Modals

Triggered by "View Session →" buttons throughout the app. Each lift modal contains:
- Session name, focus areas, duration
- Travel mode banner (if not Home) with substitution context
- Phase-specific notes (bench progression status, landmine rotation prescription, conditioning format)
- Maintenance phase notice (Phase 4–5 compounds)
- Full exercise list with:
  - Exercise order code (A1, B2, F1, etc.)
  - Exercise name with phase-aware badges (bench progression, landmine)
  - Sets and rep prescription
  - Coaching notes
  - **Weight input field** — number input in lbs, 2.5 lb step increments, persists per week/session/gym mode
  - **"Done as prescribed" checkbox** — per exercise, independent of session-level completion
- **Session notes textarea** — free text, saves on every keystroke via oninput, persists per week per session
- Delt finisher reminder

### Persistence Model

All data stored in localStorage under key `hybrid-gorilla-v2`.

| Key Pattern | Type | Description |
|-------------|------|-------------|
| `done-{week}-{dow}-{sessionKey}` | boolean | Session-level completion |
| `ex-{week}-{liftKey}-{gymMode}-{ord}-w` | string | Per-exercise weight (lbs) |
| `ex-{week}-{liftKey}-{gymMode}-{ord}-d` | boolean | Per-exercise done checkbox |
| `notes-lift-{liftKey}-w{week}` | string | Session free-text notes |
| `tt-{week}` | string | Time trial result |

---

## Equipment

| Item | Role in Program |
|------|----------------|
| Squat rack | Safety bar squat, barbell bench (Ph 3+), weighted pull-up |
| **Olympic barbell** | Bench press (Ph 3+), Romanian deadlift, overhead press |
| Dumbbells (up to 90 lbs/side) | Bench (Ph 1–2), all DB movements, delt finisher, conditioning, travel |
| Safety bar (SSB) | Lower A1 — reduces anterior torque vs. straight bar |
| **Landmine attachment** | Upper A B1 press + B2 row, Lower F1 rotation, Conditioning B1 squat-to-press + B3 rotation |
| Cables (high + low pulley) | Lateral raises, face pulls, rear delt flies, tricep pushdown, cable crunch, pull-through |
| Flat bench + incline bench | Bench press, dumbbell pressing movements |
| Dip station | Upper B weighted dip |
| Pull-up bar | Weighted pull-up (Upper A), hanging leg raise (abs) |
| Nordic curl / Roman chair bench | Lower A2 Nordic curl, Lower B2 back extension |
| TRX system | Ab fallout/pike, travel pull movements |
| **Trap bar** | Conditioning Day farmer holds (Ph 3–5) |
| **Weighted vest** | Conditioning Day burpee EMOM (Ph 4–5) |
| Peloton Tread | All running — easy, quality, long, time trials |

**Travel Best Case:** Adjustable DBs to ~60 lbs + cable stack  
**Travel Worst Case:** Fixed DBs to ~30 lbs + treadmill only

---

## Foundational Sources & Philosophy

### Resistance Training

**RP Scientific Principles of Hypertrophy Training** (Renaissance Periodization)  
Dr. Mike Israetel · Dr. James Hoffmann · Dr. Melissa Davis

Key principles applied to this program:
- MEV/MAV: sets per muscle week targeted in quality-gated ranges, expanding across phases
- RIR framework: every work set gauged by proximity to failure on a 0–4 scale
- Mechanical tension as primary driver: full ROM, controlled eccentrics, explosive concentrics
- Progressive overload via logbook: every session references the previous session
- Frequency ~2× per week per muscle
- Mandatory deloads every 8 weeks

**J3 University X Frame Hypertrophy Program** (John Jewett, IFBB Pro)

Key adaptations applied:
- X Frame priority: lateral delts, rear delts, back width, and legs structurally prioritized
- Session ordering: priority muscles trained first while neurologically fresh
- Set intensifiers: drop sets and rest-pause introduced in Weeks 6–7 before each deload
- Daily waist training adapted to 10–12 min comprehensive core session
- Exercise selection philosophy: find the movement with the strongest mind-muscle connection; rotate if needed

### Running

**Daniels' Running Formula** (Jack Daniels, Ph.D.)

Built on the VDOT framework — the most rigorously evidence-based system for distance running training. Training intensities (E/T/I/R) prescribed in Peloton mph rather than min/mile pace, since the Peloton Tread displays speed. VO2max 52 → VDOT ~53 → predicted 5K ~18:15. Gap from current 21:00 to ceiling is specific endurance and running economy — both highly trainable over 36 weeks.

---

## Technical Notes

- Single HTML file — 1,600+ lines, ~125KB uncompressed
- Zero external dependencies (Google Fonts CDN only — Oswald, Manrope, JetBrains Mono)
- All persistence via localStorage, key `hybrid-gorilla-v2`
- Mobile-first, designed and tested at 393px viewport (iPhone 14 Pro)
- PWA-ready: `apple-mobile-web-app-capable` and `apple-mobile-web-app-status-bar-style` meta tags set
- **Action registry pattern:** onclick handlers use a global `regAction(fn)` / `triggerAction(key)` registry rather than `fn.toString()` — prevents object serialization failures in template literals
- **Gym mode state** (`home` / `travel-best` / `travel-worst`): stored in memory, resets on page load — intentional so travel mode does not persist unexpectedly across sessions
- Exercise weight and completion data keyed by `week + session + gym mode`: home and travel logs stored independently and never overwrite each other
- Program start date hardcoded: April 27, 2026
- Race date hardcoded: December 31, 2026
- Total program days: 249 (TOTAL_DAYS constant)
- Total weeks: 36 (Week 36 = Dec 28–31, short 4-day race week)
- Phase boundaries, deload weeks, and time trial checkpoints derived from program start date at runtime — no hardcoded per-week data
- Storage key versioned (`v2`) to avoid conflicts with v1.0 data

---

## Credits & Sources

- **RP Scientific Principles of Hypertrophy Training** — Renaissance Periodization (Dr. Mike Israetel, Dr. James Hoffmann, Dr. Melissa Davis)
- **J3 University X Frame Hypertrophy Program** — John Jewett (J3University.com)
- **Daniels' Running Formula** — Jack Daniels, Ph.D. (VDOT framework, training zone definitions)
- Supplement protocol: evidence-based recommendations derived from published peer-reviewed research on creatine, beta-alanine, citrulline, leucine, carnitine, and betaine supplementation in trained athletes
- Program design, v1.0 build, v2.0 full rebuild and all subsequent iterations: built with Claude (Anthropic), April 2026

---

*"The hallmark of a champion physique begins with the structure of an X frame."* — J3U  
*"The goal of every easy run is to arrive at the next hard run ready to run hard."* — Jack Daniels
