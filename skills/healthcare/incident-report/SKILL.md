---
name: incident-report
version: 1.0.0
released: 2026-09-05
description: >
  Structures a clinical incident, near-miss, or hazard report into a
  factual timeline, contributing factors, and immediate actions taken —
  from a free-text account, verbal description, or rough notes. Leaves
  severity rating, root-cause classification, and any disciplinary
  judgement to the reporter and reviewer. Trigger when a clinician or ward
  manager needs to write up an incident, near miss, or hazard for the
  facility's reporting system.
keywords:
  content-type: Clinical Documentation
  thematic-category: Clinical Communication And Safety
  use-case-theme: Clinical Communication And Safety
  use-case:
    - Incident Reporting
    - Patient Safety
    - Quality Improvement
  topics: Incident Reporting
  keyword:
    - Incident Report
    - Near Miss
    - Root Cause Analysis
    - Clinical Safety
    - Contributing Factors
references:
  - "Agency for Healthcare Research and Quality (AHRQ), Common Formats"
  - "Australian Commission on Safety and Quality in Health Care (ACSQHC)"
  - "World Health Organization, Conceptual Framework for the International Classification for Patient Safety"
---

# Incident Report Writer

An incident report is only useful if it reconstructs what actually happened
clearly enough for someone who wasn't there to understand it — and keeps
fact separate from judgement. This skill turns a free-text account into a
factual, timeline-based report. It never assigns severity, blame, or root
cause — those calls belong to the reporter and the review committee.

---

## What this skill needs

- The free-text or verbal account of what happened.
- The facility's report template or fields, if there is one — ask if unclear.
- Patient/staff identifiers per your service's de-identification convention.

---

## Step 1: Extract the factual timeline

Reconstruct a chronological sequence of what happened, who was involved (by
role, not judgement — "the attending nurse," not "the negligent nurse"), and
when each event occurred, using only what's stated. Mark timing as
"approximate" rather than guessing precision the source doesn't have.

**Completion criterion:** every event in the account appears in the timeline
in order, with uncertain timing marked as approximate.

---

## Step 2: Separate fact from interpretation

Pull contributing factors out as neutral observations — "the call bell was
out of reach" — not conclusions — "nursing was negligent." Anything that
reads as a judgement rather than an observation gets flagged back to the
reporter to confirm or rephrase.

**Completion criterion:** no sentence in the contributing-factors section
assigns blame or names a cause; anything ambiguous is flagged rather than
resolved.

---

## Step 3: Draft the report

Use the facility's structure if supplied; otherwise: what happened,
contributing factors, immediate actions taken, immediate risk mitigation,
follow-up required. Leave severity rating and root-cause fields blank or
marked for the reporter/reviewer to complete.

**Completion criterion:** the draft has no severity rating or causal
conclusion the source account didn't already state.

---

## Output format

Match the facility's template fields if supplied. Otherwise, the structure
above — each section 2–5 sentences, timeline as a bulleted, timestamped
list.

---

## Gotchas

- Never assigns a severity rating, harm score, or root-cause classification
  — these require judgement and process (e.g. a formal root cause analysis)
  beyond what's in the raw account.
- Flags ambiguity in the account rather than inferring what "probably"
  happened.

---

## Evidence base

- AHRQ Common Formats — backs separating factual event description from
  causal/severity judgement, and structuring by timeline plus contributing
  factors.
- ACSQHC — backs incident reporting as a systems-focused, non-punitive
  process; this skill supports that by keeping the factual write-up free of
  blame language.
- WHO Conceptual Framework for the ICPS — the distinction between a
  "contributing factor" (an observed fact) and a "root cause" (an
  analytical conclusion) that Step 2 relies on.
