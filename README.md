# 🦍 HYBRID GORILLA v2.0

**A 36-week integrated training program for the runner who lifts.**

Built for: Steve Ricci · Age 43 · VO2max 52 · RHR 45 bpm · HRV ~70  
Goal: Sub-18:00 three-mile time trial by **December 31, 2026**  
Program start: **Monday, April 27, 2026**  
Current baseline: ~21:00 (7:00/mi · 8.57 mph)

---

## What This Is

Hybrid Gorilla is a single-file, mobile-first progressive web app that delivers a complete 36-week hybrid training program — running and resistance training fully integrated into one weekly schedule. It lives in one self-contained HTML file with no dependencies, no backend, no framework. All data (completion tracking, session notes, time trial results) is stored in the browser via localStorage.

The program bridges two worlds that are typically programmed in isolation: evidence-based hypertrophy methodology from the resistance training literature, and structured endurance running methodology from the Jack Daniels / VDOT framework. The result is a program where neither discipline cannibalizes the other — each is allocated volume and intensity based on its recovery cost relative to the shared recovery budget of a 43-year-old hybrid athlete.

---

## v2.0 Changes (April 2026)

The following enhancements were made from v1.0:

### Lift Program Overhaul

**Equipment additions recognized:** Olympic barbell + landmine attachment added to home gym alongside dumbbells (up to 90 lbs/side), safety bar, cables, pull-up/dip station, TRX, and Peloton Tread.

**Upper A (Monday) — changes:**
- **Flat Bench Progression:** DB bench (Phases 1–2) → Olympic barbell bench (Phase 3+). Phase 1–2 focus on ROM, control, and connective tissue preparation at 3×8–12. Phase 3+ transitions to barbell at 8–12 reps before resuming progressive overload. Joint and tendon health prioritized over early barbell loading.
- **B1 — Landmine Press (single-arm):** Replaces DB/cable incline press. Shoulder-friendly pressing angle, hits upper chest + anterior delt + rotational stability.
- **B2 — Landmine Row (single-arm):** Replaces chest-supported DB row. Natural arc reduces wrist strain vs. DB; same mid-back stimulus with easier setup.
- **D2 — DB Curl:** Added as a bicep movement paired with D1 (tricep pushdown). Biceps now trained twice weekly (Upper A + Upper B).

**Lower (Wednesday) — changes:**
- **B1 — Romanian Deadlift:** Upgraded to Olympic barbell as primary implement for heavier progressive loading.
- **F1 — Landmine Core Rotation (NEW):** Added as a power finisher. Fills the missing rotational pattern alongside the existing anti-extension and flexion core work. Phase-progressed volume: 2×8–10/side (Ph 1) → 2×10–12/side (Ph 2) → 3×12–15/side (Ph 3–5).

**Upper B (Friday, Phases 1–2) — changes:**
- **A1 — Barbell Overhead Press:** Upgraded to Olympic bar from DB.
- **C3 — Removed:** Behind-the-back cable lateral raise removed. Lateral delt volume remains adequate between C1 (lean-away cable lateral), Upper A, and the delt finisher.
- **D1 — DB Curl:** EZ-bar replaced with DB curl (no EZ-bar in home gym).

**Conditioning Day (Friday, Phases 3–5) — NEW:**
- Replaces Upper B when lifting drops to 2 days/week.
- Burpee-anchored full-body conditioning circuit.
- Includes: Swimmer's curls, landmine squat-to-press, landmine core rotation, farmer carry/core finisher.
- Full session design specified in app. ~35–40 min.

### Landmine Core Rotation — Program-Wide
The landmine rotation addresses the missing rotational movement pattern (existing core: anti-extension + flexion only). Placed strategically on Lower day as a power finisher (not daily — neurological demand too high for daily programming). Also featured on Conditioning Day (Fri, Ph 3–5). Intentionally excluded from Upper A (already uses landmine twice: press + row) and the daily abs session (designed for endurance-focused volume).

### Date Reset
- **New start date:** Monday, April 27, 2026 (Day 1)
- **New race date:** Thursday, December 31, 2026
- **Total program:** 249 days · 36 weeks (Week 36 = Dec 28–31, short race week)
- All phase dates, time trial checkpoints, and in-app countdowns updated accordingly.

---

## Foundational Sources & Philosophy

### Resistance Training — Source Material

**1. RP Scientific Principles of Hypertrophy Training (Renaissance Periodization)**  
Authors: Dr. Mike Israetel, Dr. James Hoffmann, Dr. Melissa Davis

Key principles applied:
- **MEV/MAV:** Sets per muscle per week targeted 8–15 (Ph 1), expanding to 12–20 (Ph 2). Volume is quality-gated — sets not approaching failure are not counted.
- **RIR (Reps in Reserve):** Every work set gauged by proximity to failure 0–4. Progresses from RIR 2 (Week 1) toward RIR 0–1 by Week 5, with mandatory deload at Week 8 (RIR 3, half volume).
- **Mechanical Tension as Primary Driver:** Full ROM, controlled eccentrics (2–3 sec), explosive concentrics.
- **Progressive Overload via Logbook:** More reps at same weight, or same reps at more weight — every session.
- **Frequency ~2x/week per muscle:** Each muscle trained approximately twice weekly.
- **Deload Protocol:** Every 8 weeks. Sets halved, loads maintained, RIR raised to 3.

**2. J3 University X Frame Hypertrophy Program (John Jewett)**  
Author: John Jewett (IFBB Pro, Olympia competitor)

Key adaptations:
- **X Frame Priority:** Lateral delts, rear delts, back width, and legs prioritized structurally.
- **Session ordering:** Delt-first on push days, lat-first on pull days, quad-first on leg days.
- **Set intensifiers:** Drop sets and rest-pause introduced in Weeks 6–7 of each phase.
- **Daily core (adapted):** J3U waist training adapted to 10–12 min daily abs session (hanging leg raise, cable crunch, ab wheel/TRX, RKC plank).

---

### Running — Source Material

**VDOT Framework (Jack Daniels, Ph.D.)**

VO2max 52 → VDOT ~53 → predicted 5K ~18:15. Gap between current 21:00 and predicted ceiling is specific endurance, running economy, and neuromuscular tolerance — all highly trainable.

| Zone | Description | mph (Peloton) | Purpose |
|------|-------------|---------------|---------|
| Easy (E) | Conversational, nasal breathing | 7.7–8.4 | Aerobic base, recovery |
| Threshold (T) | Comfortably hard, ~1hr race pace | 9.0–9.5 | Lactate threshold elevation |
| Interval (I) | 5K race effort, VO2max stimulus | 9.5–10.5 | Raise aerobic ceiling |
| Repetition (R) | Fast, short, full recovery | 10.5–11.5 | Running economy, neuromuscular sharpness |

**Goal Pace:** 10.0 mph (6:00/mi) — sustain for 18:00.

**Weekly run structure:**
- Tuesday: Threshold quality session
- Thursday: VO2max / interval quality session
- Saturday: Long aerobic run (50–90 min, phase-dependent)
- Mon/Wed/Fri: Easy runs (30–45 min) paired with lift days

---

## Program Architecture

### Phase Structure

| Phase | Weeks | Dates | Lift Days | Key Benchmark |
|-------|-------|-------|-----------|---------------|
| 1: Foundation | 1–8 | Apr 27 – Jun 21 | Mon/Wed/Fri | TT Jun 20: 20:00–20:30 |
| 2: Volume Bump | 9–16 | Jun 22 – Aug 16 | Mon/Wed/Fri | TT Aug 15: 18:45–19:15 |
| 3: Transition | 17–24 | Aug 17 – Oct 11 | Mon/Wed/Fri* | TT Oct 3: 18:30 |
| 4: Peak Running | 25–32 | Oct 12 – Dec 6 | Mon/Wed/Fri* | TT Nov 28: 18:10–18:25 |
| 5: Sharpen & Race | 33–36 | Dec 7 – Dec 31 | Mon/Wed/Fri* | **Race Dec 31: Sub-18** |

*Phase 3–5 Friday = Conditioning Day (not Upper B)

### Weekly Schedule

| Day | Phase 1–2 | Phase 3–5 |
|-----|-----------|-----------|
| Mon | Upper A + Easy Run | Upper A + Easy Run |
| Tue | Quality Run + Delt Finisher + Abs | Quality Run + Delt Finisher + Abs |
| Wed | Lower + Easy Run | Lower + Easy Run |
| Thu | Quality Run + Delt Finisher + Abs | Quality Run + Delt Finisher + Abs |
| Fri | Upper B + Easy Run | **Conditioning Day** + Easy Run |
| Sat | Long Run + Delt Finisher (optional) | Long Run + Delt Finisher (optional) |
| Sun | Rest / Thunder 45 | Rest / Thunder 45 |

---

## Lift Sessions

### Upper A — Monday (All Phases)
*Chest · Back · Lateral Delt · Rear Delt · Arms · ~50 min*

| # | Exercise | Sets × Reps | Notes |
|---|----------|-------------|-------|
| A1 | DB Bench → BB Bench (see progression) | 3 × 8–12 / 6–10 | Phase-based (see below) |
| A2 | Weighted Pull-Up or Lat Pulldown | 3 × 6–10 | |
| B1 | Landmine Press (single-arm) | 2 × 10–12/arm | |
| B2 | Landmine Row (single-arm) | 2 × 10–12/arm | |
| C1 | Low Cable Lateral Raise | 4 × 12–15 | Phase 2+: 5 sets |
| C2 | Cable Face Pull (rear delt) | 3 × 15–20 | |
| D1 | Tricep Cable Pushdown | 2 × 10–15 | Superset w/ D2 |
| D2 | DB Curl (standing or incline) | 2 × 10–12 | Superset w/ D1 |

**Flat Bench Progression:**
- **Phase 1 (Wks 1–8):** DB flat bench · 3×8–12 · ROM, control, eccentric focus
- **Phase 2 (Wks 9–16):** DB flat bench · 3×6–10 · Load toward 75–90lb DBs
- **Phase 3 (Wks 17–24):** Olympic barbell · 3×8–12 · Drop load, rebuild mechanics
- **Phase 4–5 (Wks 25–36):** Olympic barbell · 3×6–10 · Progressive overload to race day

### Lower — Wednesday (All Phases)
*Posterior Chain · Nordic Curl · Single Leg · Calves · Rotational Core · ~50 min*

| # | Exercise | Sets × Reps | Notes |
|---|----------|-------------|-------|
| A1 | Safety Bar Squat | 3 × 6–10 | |
| A2 | Nordic Curl (modified eccentric) | 3 × 4–6 ecc | 5-count descent |
| B1 | Romanian Deadlift (Olympic bar) | 3 × 6–10 | |
| B2 | Roman Chair Back Extension | 3 × 10–15 | |
| C1 | Rear-Foot-Elevated Split Squat (DB) | 2 × 8–10/leg | |
| D1 | Standing Calf Raise (bar or DB) | 3 × 8–12 | |
| D2 | Cable Pull-Through or Hip Thrust | 2 × 10–15 | |
| E1 | Copenhagen Plank or Cable Adductor | 2 × 30s / 10–15 | |
| F1 | **Landmine Core Rotation** | 2–3 × 8–15/side | Phase-progressed |

**Landmine Core Rotation Progression:**
- Phase 1: 2×8–10/side · light load · technique focus
- Phase 2: 2×10–12/side · moderate load
- Phase 3–5: 3×12–15/side · rotational power emphasis

### Upper B — Friday (Phases 1–2 only)
*Shoulders · Lateral Delt · Rear Delt · Back · Arms · ~50 min*

| # | Exercise | Sets × Reps | Notes |
|---|----------|-------------|-------|
| A1 | Barbell OHP (Olympic bar, strict) | 3 × 6–10 | |
| A2 | Chin-Up or Supinated Cable Pulldown | 3 × 6–10 | |
| B1 | Weighted Dip (or DB Floor Press) | 2 × 8–12 | |
| B2 | Single-Arm Cable Row (half-kneeling) | 2 × 10–12/arm | |
| C1 | Lean-Away Cable Lateral Raise | 4 × 12–15 | Phase 2+: 5 sets |
| C2 | Rear Delt Cable Fly (high pulley) | 3 × 15–20 | |
| D1 | DB Curl (preacher or standing) | 2 × 10–12 | Superset w/ D2 |
| D2 | Overhead DB Tricep Extension | 2 × 10–12 | Superset w/ D1 |

### Conditioning Day — Friday (Phases 3–5)
*Full-Body · Burpee Anchor · Landmine Power · Metabolic · ~35–40 min*

Replaces Upper B when lifting drops to 2 dedicated days. Maintains athletic conditioning and complements the running priority of the back half of the program.

| # | Exercise | Notes |
|---|----------|-------|
| A | Burpee EMOM or Timed Sets | Primary conditioning anchor; volume progresses Ph 3–5 |
| B | Swimmer's Curl (DB) | Full shoulder arc, anterior chain, compound curl |
| C | Landmine Squat-to-Press | Full-body power; hip drive transfers through core to press |
| D | Landmine Core Rotation | Consistent with Lower day F1 — rotational power block |
| E | Farmer Carry or Core Finisher | Session cap; grip + gait + mental toughness |

---

## Delt Priority

Weekly lateral and rear delt volume:
- **Upper A:** 4–5 sets lateral (C1), 3 sets rear (C2)
- **Upper B (Ph 1–2):** 4–5 sets lateral (C1), 3 sets rear (C2)
- **Delt Finisher (Tue/Thu/Sun + opt. Sat):** 2–3 sets lateral, 2–3 sets rear, 2–3 sets shrug (Ph 1–2); +band pull-apart Ph 3–5
- **Total: ~12–22 sets lateral, ~10–18 sets rear per week** across phases

Angle variation: low cable (Upper A, front angle), lean-away cable (Upper B, neutral/elongated), daily finisher (both).

---

## Nordic Curl Progression

Programmed Lower day A2 throughout all 36 weeks. #1 evidence-based hamstring injury prevention for runners.
- Phase 1–2: Modified Nordic (reduced range, 5-count eccentric, hands ready to catch)
- Phase 3+: Fuller range as strength and tendon tolerance develop

---

## Core / Abs Session (Daily)

10–12 minutes. Separate from lift sessions when possible.

| # | Exercise | Sets × Reps | Pattern |
|---|----------|-------------|---------|
| 1 | Hanging Leg Raise | 3 × 8–12 | Flexion |
| 2 | Cable Crunch (rope) | 3 × 10–15 | Flexion |
| 3 | Ab Wheel Rollout or TRX Fallout | 2 × 8–12 | Anti-extension |
| 4 | RKC Plank | 2 × 20–30s | Full-body irradiation |

TRX alternatives toggle in-app. Ab vacuums performed opportunistically throughout the day.

---

## Recovery Philosophy

Recovery is the limiting variable — not training stress. Stimulus you cannot recover from is negative stimulus.

- **Sleep:** 7–8 hrs/night. Non-negotiable.
- **No lower body lifting within 48 hrs before Thursday VO2 session.**
- **No lower body lifting the day before Saturday long run.**
- **Nutrition:** Maintenance or very slight surplus (~100–200 cal above TDEE). 1.0–1.2g protein/lb. 2.5–4g carbs/lb on training days.
- **Deloads:** Mandatory at Weeks 8, 16, 24, 32. Sets halved, loads maintained, RIR 3.

**Bad Day Protocol:** If 2+ of — poor recovery, bad sleep, elevated stress, missed meals, joint pain — cut to 1 set per exercise at RIR 2–3. Downgrade quality runs to easy fartlek.

---

## Travel Training

Two tracks toggled in-app:

**Best Case** (cable stack + adjustable DBs to ~60 lbs): Full program replication with cable laterals, DB compounds, floor-based Nordics.

**Worst Case** (fixed DBs max ~30 lbs + treadmill): Unilateral emphasis (single-leg RDL, split squat), higher-rep ranges, technique-intensive movements (archer push-up, lean-away DB lateral, prone Y-raise).

---

## App Features

- **Today view:** Current day's full session stack with completion checkboxes
- **Week view:** 7-day overview with session labels, navigate any week
- **Plan view:** Full 36-week arc by phase, current week auto-highlighted
- **Paces view:** Speed zones in Peloton mph, training zone crosswalk, time trial log
- **Session modals:** Full exercise list with sets, reps, coaching notes, phase-aware bench badge, landmine badges
- **Progress bar:** Tracks completion across 249 total program days
- **Race countdown:** Days until December 31, 2026 in header

---

## Time Trial Checkpoints

| Week | Date | Target |
|------|------|--------|
| 0 | Apr 27, 2026 | Baseline: ~21:00 |
| 8 | Jun 20, 2026 | 20:00–20:30 |
| 16 | Aug 15, 2026 | 18:45–19:15 |
| 23 | Oct 3, 2026 | 18:30 |
| 31 | Nov 28, 2026 | 18:10–18:25 |
| **36** | **Dec 31, 2026** | **Sub 18:00** |

---

## Equipment

**Home gym:**
- Squat rack, Olympic barbell, dumbbells (up to 90 lbs/side), safety bar (SSB)
- **Landmine attachment** (used on: Upper A press + row, Lower rotation, Conditioning Day)
- Cables: high pulley, low pulley, adjustable
- Bench, incline bench
- Dip station, pull-up bar
- Nordic curl / Roman chair hyperextension bench
- TRX system
- Peloton Tread

**Travel (best case):** Adjustable DBs to ~60 lbs, cable stack  
**Travel (worst case):** Fixed DBs to ~30 lbs, treadmill only

---

## Technical Notes

- Single HTML file, ~90KB uncompressed
- No external dependencies (Google Fonts CDN only)
- localStorage for all persistence (completion, notes, TT results)
- Storage key: `hybrid-gorilla-v2`
- Mobile-first, tested at 393px width (iPhone 14 Pro viewport)
- Designed for Safari "Add to Home Screen" installation
- Program start date: April 27, 2026
- Race date: December 31, 2026
- Total program: 249 days / 36 weeks

---

## Credits & Sources

- **RP Scientific Principles of Hypertrophy Training** — Renaissance Periodization (Dr. Mike Israetel, Dr. James Hoffmann, Dr. Melissa Davis)
- **J3 University X Frame Hypertrophy Program** — John Jewett (J3University.com)
- **Daniels' Running Formula** — Jack Daniels, Ph.D. (VDOT framework, training zone definitions)
- Program design, v1.0 build, and v2.0 enhancements: built with Claude (Anthropic), April 2026

---

*"The hallmark of a champion physique begins with the structure of an X frame."* — J3U  
*"The goal of every easy run is to arrive at the next hard run ready to run hard."* — Jack Daniels
