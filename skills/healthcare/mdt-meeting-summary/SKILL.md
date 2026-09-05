---
name: mdt-meeting-summary
version: 1.0.0
released: 2026-09-05
description: >
  Structures a multidisciplinary team (MDT) meeting, ward round, or case
  conference — from a transcript, notes, or dictation — into a clean
  summary with per-patient care decisions, actions, and owners. Trigger
  when a clinician or coordinator needs minutes from an MDT meeting, tumour
  board, case conference, or ward round.
keywords:
  content-type: Clinical Documentation
  thematic-category: Clinical Communication And Safety
  use-case-theme: Clinical Communication And Safety
  use-case:
    - Care Coordination
    - Multidisciplinary Teamwork
    - Meeting Documentation
  topics: Care Coordination
  keyword:
    - MDT Meeting
    - Case Conference
    - Ward Round
    - Care Plan Actions
    - Tumour Board
references:
  - "Australian Commission on Safety and Quality in Health Care (ACSQHC)"
  - "NHS England, Multidisciplinary Team guidance"
  - "World Health Organization, Framework on Integrated People-Centred Health Services"
---

# MDT Meeting Summary

An MDT meeting has done its job when every patient discussed leaves with a
clear, owned next step — not just a record that they were talked about.
This skill turns a transcript, dictation, or rough notes into a per-patient
summary built around decisions and actions, not a general discussion log.

---

## What this skill needs

- The transcript, dictation, or notes from the meeting.
- The list of patients/cases covered, if not obvious from the notes.

---

## Step 1: Segment by patient

Break the raw notes into one block per patient discussed, in the order they
came up.

**Completion criterion:** every patient named in the source material has
their own block.

---

## Step 2: Capture discussion, decision, and action

For each patient, extract:

- **Discussion** — a one- to two-sentence summary of what was covered.
- **Decision** — what the team actually decided, stated plainly.
- **Action** — what happens next, who owns it, and by when.

**Completion criterion:** every patient block has a stated decision (or "no
decision reached") and, where a decision was made, an action with an owner.

---

## Step 3: Flag unresolved cases

Where a patient was discussed without a clear decision or action, mark it
for follow-up at the next meeting rather than inventing a plausible-sounding
outcome.

**Completion criterion:** no patient block shows a decision or action that
wasn't actually stated in the source material.

---

## Output format

One block per patient: **Patient** | **Discussion** | **Decision** |
**Action** (owner, by when).

---

## Gotchas

- This documents what the team decided — it does not make or suggest
  clinical decisions itself.

---

## Evidence base

- ACSQHC, Comprehensive Care Standard — backs documenting a clear, owned
  care-plan action per patient rather than a discussion record.
- NHS England, Multidisciplinary Team guidance — backs the
  decision-plus-action-plus-owner structure as the actual point of MDT
  documentation, not the discussion itself.
- WHO, Framework on Integrated People-Centred Health Services — backs
  continuity across disciplines as the reason a structured hand-off from
  the meeting to the ward matters.
