---
name: okr-check-in
version: 1.0.0
released: 2026-09-05
description: >
  Turns raw progress notes into a structured OKR or goal check-in —
  progress against each key result, a confidence score with a reason, and
  named blockers — in the format a team or leadership review expects.
  Trigger when someone needs an OKR update, goal check-in, or quarterly
  progress summary against key results.
keywords:
  content-type: Goal Check-In
  thematic-category: Workplace Operations And Communication
  use-case-theme: Workplace Productivity And Communication
  use-case:
    - Goal Tracking
    - Team Communication
    - Performance Management
  topics: OKR Reporting
  keyword:
    - OKR Check-In
    - Key Results
    - Confidence Score
    - Goal Tracking
    - Quarterly Review
references:
  - "John Doerr, Measure What Matters"
  - "Google re:Work, OKR guidance"
---

# OKR Check-In

A confidence score with no reason attached is a guess dressed up as data.
This skill's discipline is attaching a stated reason to every score, and
naming the specific blocker behind anything below target — not a vague
"behind schedule."

---

## What this skill needs

- The objective and key results as set.
- Raw progress notes for the period.

---

## Step 1: Score each key result

For each key result, state the current value against target and a
confidence score (0.0–1.0, or red/amber/green) based on what the notes
actually support — not an optimistic default.

**Completion criterion:** every key result has a stated current value and a
confidence score with a one-line reason.

---

## Step 2: Name blockers

Where confidence is below target, name the specific blocker rather than a
generic "behind schedule" or "in progress."

**Completion criterion:** every below-target key result has a named,
specific blocker, not a restatement of the low score.

---

## Step 3: Note the path back, if given

If the owner's notes state what would need to change to get back on track,
include it. Don't invent a recovery plan they didn't give.

**Completion criterion:** any recovery plan in the output was present in the
source notes, not generated to fill the gap.

---

## Output format

Per key result: Target | Current | Confidence (with reason) | Blocker (if
below target) | Path back (if stated).

---

## Gotchas

- A confidence score with no reason is a guess dressed as data — always
  attach the one-line reason.

---

## Evidence base

- Doerr, *Measure What Matters* — backs the confidence-scored check-in
  (rather than percent-complete alone) as the OKR-review discipline, since
  it surfaces risk before the quarter ends rather than at the deadline.
- Google re:Work OKR guidance — backs naming specific blockers over generic
  "on track/behind" framing.
