# 🦍 HYBRID GORILLA

**A 36-week integrated training program for the runner who lifts.**

Built for: Steve Ricci · Age 43 · VO2max 52 · RHR 45 bpm · HRV ~70  
Goal: Sub-18:00 three-mile time trial by **December 26, 2026**  
Current baseline: ~21:00 (7:00/mi · 8.57 mph)

---

## What This Is

Hybrid Gorilla is a single-file, mobile-first progressive web app that delivers a complete 36-week hybrid training program — running and resistance training fully integrated into one weekly schedule. It lives in one self-contained HTML file with no dependencies, no backend, no framework. All data (completion tracking, session notes, time trial results) is stored in the browser via localStorage.

The program bridges two worlds that are typically programmed in isolation: evidence-based hypertrophy methodology from the resistance training literature, and structured endurance running methodology from the Jack Daniels / VDOT framework. The result is a program where neither discipline cannibalizes the other — each is allocated volume and intensity based on its recovery cost relative to the shared recovery budget of a 43-year-old hybrid athlete.

---

## Foundational Sources & Philosophy

### Resistance Training — Source Material

The lifting side of this program is built directly on two source documents:

**1. RP Scientific Principles of Hypertrophy Training (Renaissance Periodization)**  
Authors: Dr. Mike Israetel, Dr. James Hoffmann, Dr. Melissa Davis  
This text establishes the evidence-based framework for muscle hypertrophy programming. Key principles extracted and applied:

- **Minimum Effective Volume (MEV) and Maximum Adaptive Volume (MAV):** Sets per muscle per week are targeted in the 8–15 range in Phase 1, expanding to 12–20 in Phase 2. Volume is quality-gated — sets that do not approach muscular failure are not counted toward working volume.
- **Reps in Reserve (RIR):** Every work set is gauged by proximity to concentric failure on a 0–4 scale. RIR 0 = failure reached. The program progresses from RIR 2 in Week 1 toward RIR 0–1 by Week 5, with a deliberate deload at Week 8 (RIR 3, half volume).
- **Mechanical Tension as Primary Driver:** Metabolic stress and muscle damage are secondary. The priority is creating high mechanical tension in the target muscle through full range of motion, controlled eccentrics (2–3 second lowering), and explosive concentrics.
- **Progressive Overload via Logbook:** Every session, the previous session's loads and reps are referenced. Progression is defined as: more reps at the same weight, or the same reps at more weight. Form is standardized in Week 1 and never altered to chase numbers.
- **Frequency ~2x per week per muscle:** Each muscle group is trained approximately twice per week. Upper body muscles receive the full 2x frequency. Lower body receives 1x dedicated session, with running providing the second stimulus.
- **Deload protocol:** Every 8 weeks. Sets halved, loads maintained, RIR raised to 3. Physical and neurological recovery. Not optional.

**2. J3 University X Frame Hypertrophy Program (John Jewett)**  
Author: John Jewett (IFBB Pro, Olympia competitor)  
This program provides the structural template and in-the-trenches application of the RP principles. Key adaptations:

- **X Frame Priority:** The program structurally prioritizes the four pillars of an X frame physique — wide lats, capped delts, sweeping quads, small waist. For a non-competitor, this translates to prioritizing delts (lateral and rear head), back width, and legs.
- **Session structure:** Push days are delt-first (lateral raises before pressing). Pull days are lat-first (pulldown before rows). Leg days are quad-first. This ordering ensures the priority muscles receive the highest quality stimulus when neurological freshness is highest.
- **Set intensifiers:** Drop sets and rest-pause sets are introduced in Weeks 6–7 of each phase — not as a permanent fixture, but as a peak-stimulus tool leading into the deload.
- **Daily waist training (adapted):** The J3U protocol prescribes daily ab vacuums and contractions. This program adapts that into a dedicated 10–12 minute daily core session (hanging leg raises, cable crunches, ab wheel/TRX fallout, RKC plank) with vacuums performed opportunistically throughout the day rather than in a formal session.
- **Exercise selection philosophy:** Exercises are suggestions, not mandates. The principle is finding the movement that creates the strongest mind-muscle connection in the target muscle. If a lift isn't progressing or isn't felt in the right place, it gets rotated out.

---

### Running — Source Material & Framework

The running side is built on the **Jack Daniels VDOT Running Formula** — the most rigorously evidence-based framework for distance running training.

**VDOT Framework (Jack Daniels, Ph.D.)**  
A VO2max of 52 predicts a VDOT of approximately 53, corresponding to a 5K time of ~18:15. The athlete's current 3-mile time of 21:00 sits well below their predicted ceiling, indicating that the gap is not aerobic capacity but specific endurance, running economy, and neuromuscular tolerance of goal pace — all highly trainable.

The four training intensities used:

| Zone | Description | mph (Steve's scale) | Purpose |
|------|-------------|---------------------|---------|
| Easy (E) | Conversational, nose breathing | 7.7–8.4 | Aerobic base, recovery |
| Threshold (T) | Comfortably hard, ~1hr race pace | 9.0–9.5 | Lactate threshold elevation |
| Interval (I) | 5K race effort, VO2max stimulus | 9.5–10.5 | Raise aerobic ceiling |
| Repetition (R) | Fast, short, full recovery | 10.5–11.5 | Running economy, neuromuscular sharpness |

**Goal Pace** sits at exactly 10.0 mph (6:00/mi) — the top of the athlete's self-reported "challenging" zone. Sub-18:00 requires sustaining this for 18 minutes. The program's running prescription systematically makes 10.0 mph feel easier by:
1. Raising threshold pace toward goal pace (T work)
2. Building tolerance for faster-than-goal pace in short reps (I and R work)
3. Increasing time-at-goal-pace exposure over 36 weeks

**Weekly run structure:**
- Tuesday: Threshold quality session
- Thursday: VO2max / interval quality session
- Saturday: Long aerobic run (60–100 min)
- Mon / Wed / Fri: Easy runs (30–45 min) with optional strides

---

## Program Architecture

### Phase Structure

| Phase | Weeks | Dates | Lift Days | Running Focus | Key Benchmark |
|-------|-------|-------|-----------|---------------|---------------|
| 1: Foundation | 1–8 | Apr 20 – Jun 14 | Mon/Wed/Fri | Threshold intro, VO2 fartleks | TT Wk 8: 20:00–20:30 |
| 2: Volume Bump | 9–16 | Jun 15 – Aug 9 | Mon/Wed/Fri | Goal-pace intervals introduced | TT Wk 16: 18:45–19:15 |
| 3: Transition | 17–24 | Aug 10 – Oct 4 | Mon/Wed | Running becomes priority | TT Wk 23: 18:30 |
| 4: Peak Running | 25–32 | Oct 5 – Nov 29 | Mon/Wed (maint.) | Peak volume, 5K-specific | TT Wk 31: 18:10–18:25 |
| 5: Sharpen & Race | 33–36 | Nov 30 – Dec 26 | Mon/Wed (maint.) | Taper, race-pace sharpening | **Race Dec 26: Sub-18** |

### Lift Split

**Upper A (Monday):** Horizontal push/pull emphasis — DB bench, weighted pull-up, incline press, chest-supported row, low cable lateral raise (4–5 sets), cable face pull (3 sets), tricep pushdown.

**Lower (Wednesday):** Run-supportive posterior chain — safety bar squat, Nordic curl (modified → full progression), Romanian deadlift, Roman chair back extension, rear-foot-elevated split squat, standing calf raise, cable pull-through, Copenhagen plank.

**Upper B (Friday, Phases 1–2 only):** Vertical push/pull + shoulders — overhead press, chin-up, weighted dip, single-arm cable row, lean-away cable lateral raise (4–5 sets), rear delt cable fly (3 sets), behind-the-back cable lateral raise (2 sets), curl, overhead tricep extension.

### Delt Priority

Lateral and rear deltoid development is explicitly maximized. The scientific rationale: the lateral head of the deltoid has a very short effective range of stimulus (it only generates significant mechanical tension in the top ~60° of a lateral raise), which means it responds well to high frequency, moderate volume, and varied angles. The rear delt is similarly frequency-tolerant.

**Weekly delt volume:**
- Upper A: 4 sets lateral, 3 sets rear (5/4 in Phase 2+)
- Upper B: 4 sets lateral (lean-away), 3 sets rear fly, 2 sets behind-back lateral (5/4/2 in Phase 2+)
- Delt Finisher (Tue/Thu/Sun, optional Sat): 2–3 sets lateral, 2–3 sets rear, 2–3 sets DB shrug
- **Total: ~14–24 sets lateral, ~12–20 sets rear per week** depending on phase

Angle variation is deliberate: low cable (front angle), lean-away cable (neutral), behind-back cable (posterior angle). Each hits a slightly different portion of the lateral head.

### Nordic Curl Progression

Nordic curls are programmed on the Lower day (A2, paired with safety bar squat) throughout all 36 weeks. They are the single most evidence-supported exercise for hamstring injury prevention in runners. The progression:
- Phase 1–2: Modified Nordic (reduced range, hands ready to catch, 5-count eccentric)
- Phase 3+: Fuller range as strength and tolerance build

### Core / Abs Session

Daily, 10–12 minutes. Replaces the J3U waist training protocol with a more comprehensive approach for an already-strong core:

1. Hanging leg raise — 3 × 8–12 (posterior pelvic tilt at top, full control)
2. Cable crunch (rope) — 3 × 10–15 (spinal flexion, not hip flexion)
3. Ab wheel rollout or TRX fallout — 2 × 8–12 (hollow body, anti-extension)
4. RKC Plank — 2 × 20–30s (full-body irradiation, not a rest)

TRX variations (fallout, pike, body saw) toggle on via in-app checkbox.

Ab vacuums are performed opportunistically throughout the day — desk, car, anywhere — rather than as a formal session component.

---

## Recovery Philosophy

Recovery is treated as the limiting variable — not training stress. The central insight from both the RP and J3U sources: **stimulus you cannot recover from is negative stimulus.** For a hybrid athlete running 6 days per week plus 3 lift sessions plus weekly conditioning (Thunder 45), the recovery budget is finite and must be allocated deliberately.

**Key recovery rules:**
- 7–8 hours sleep per night. Non-negotiable. The single highest-leverage recovery intervention.
- No lower body lifting within 48 hours before Thursday's VO2 session.
- No lower body lifting the day before Saturday's long run.
- Nutrition: maintenance or very slight surplus (~100–200 cal above TDEE). Aggressive surplus is counter-productive for a runner — every pound of excess body weight costs ~2 seconds per mile.
- Protein: 1.0–1.2g/lb. Carbohydrates: 2.5–4g/lb on training days. Carbs are the primary running fuel and are not restricted.
- Deloads are mandatory at Weeks 8, 16, 24, 32. Missing deloads is the most common way a program breaks down.

**Autoregulation (Bad Day Protocol):**  
If 2+ of the following are true — perceived recovery low, poor sleep, elevated stress, missed meals, joint pain — training is cut to one set per exercise at RIR 2–3 and 12–15 reps. Quality runs are downgraded to easy fartlek. The program accommodates reality.

---

## Travel Training

Two distinct tracks for travel, toggled in-app:

**Best Case** (cable stack + adjustable DBs to ~60 lbs): Full program replication with cable-based laterals, DB compound movements, floor-based Nordic curls.

**Worst Case** (fixed DBs max ~30 lbs + treadmill): Compensated via unilateral movements (single-leg RDL, split squat with front foot elevated), higher-rep ranges, technique-intensive movements (archer push-up, lean-away DB lateral raise, prone Y-raise) that generate adequate stimulus at lower absolute loads.

Both tracks maintain the delt priority. Rear delt fly and lateral raise mechanics are preserved across all equipment scenarios.

---

## App Features

- **Today view:** Current day's full session stack with completion checkboxes. Gym mode toggle (Home / Travel Best / Travel Worst) at top.
- **Week view:** 7-day overview with tap-to-expand day detail. Navigate any of the 36 weeks.
- **Plan view:** Full 36-week arc organized by phase. Current week auto-highlighted. Tap any week to jump to it.
- **Paces view:** Speed zones in mph (Peloton-native), min/mile conversion, Peloton zone → training zone crosswalk, time trial log with editable result fields.
- **Session modals:** Full exercise list with sets, reps, coaching notes. In-lift session notes field (persisted to localStorage). TRX toggle in abs modal. Delt finisher with weekly volume summary.
- **Progress tracking:** Completion checkboxes per session, persistent across sessions. Progress bar in header.
- **Race countdown:** Days until December 26, 2026 always visible in header.

---

## Time Trial Checkpoints

| Week | Date | Target |
|------|------|--------|
| 0 | Apr 20, 2026 | Baseline: 21:00 (current) |
| 8 | Jun 13, 2026 | 20:00–20:30 |
| 16 | Aug 8, 2026 | 18:45–19:15 |
| 23 | Sep 26, 2026 | 18:30 |
| 31 | Nov 21, 2026 | 18:10–18:25 |
| 36 | **Dec 26, 2026** | **Sub 18:00** |

---

## Equipment

**Home gym:**
- Squat rack, barbell, dumbbells, safety bar (SSB)
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

- Single HTML file, ~87KB uncompressed
- No external dependencies (fonts loaded from Google Fonts CDN)
- localStorage for all persistence (completion, notes, TT results)
- Storage key: `hybrid-sub18-v2`
- Mobile-first, tested at 393px width (iPhone 14 Pro viewport)
- Designed for Safari "Add to Home Screen" installation
- Program start date hardcoded: April 20, 2026
- Race date hardcoded: December 26, 2026

---

## Credits & Sources

- **RP Scientific Principles of Hypertrophy Training** — Renaissance Periodization (Dr. Mike Israetel, Dr. James Hoffmann, Dr. Melissa Davis)
- **J3 University X Frame Hypertrophy Program** — John Jewett (J3University.com)
- **Daniels' Running Formula** — Jack Daniels, Ph.D. (VDOT framework, training zone definitions)
- Program design, integration, and application: built with Claude (Anthropic), April 2026

---

*"The hallmark of a champion physique begins with the structure of an X frame."* — J3U  
*"The goal of every easy run is to arrive at the next hard run ready to run hard."* — Jack Daniels
