---
name: shift-handover-note
version: 1.0.0
released: 2026-09-05
description: >
  Structures a clinical shift handover into SBAR format (Situation,
  Background, Assessment, Recommendation) from rough notes, a verbal
  account, or a partial handover sheet — flagging any of the four sections
  left thin so nothing falls through at shift change. Trigger when a nurse,
  midwife, or allied health clinician needs to write or tidy up a handover
  note, ward round summary, or patient handoff for the incoming shift.
keywords:
  content-type: Clinical Documentation
  thematic-category: Clinical Communication And Safety
  use-case-theme: Clinical Communication And Safety
  use-case:
    - Shift Handover
    - Patient Safety
    - Care Continuity
  topics: Clinical Handover
  keyword:
    - SBAR
    - Shift Handover
    - Ward Round Summary
    - Patient Handoff
    - Care Continuity
references:
  - "World Health Organization, Patient Safety Solutions"
  - "Institute for Healthcare Improvement (IHI)"
  - "Australian Commission on Safety and Quality in Health Care (ACSQHC)"
  - "The Joint Commission"
---

# Shift Handover Note (SBAR)

Poor handover communication is one of the most consistently cited
contributing factors in preventable clinical incidents. This skill turns
rough notes, dictation, or a partial handover sheet into a complete SBAR
handover — Situation, Background, Assessment, Recommendation — so the
incoming shift has everything it needs to pick up each patient safely.

---

## What this skill needs

- The patient identifier convention your service uses (bed number, initials,
  MRN — never record identifying detail beyond what your service's own
  handover process already uses).
- Rough notes, dictation, or a partial handover sheet for each patient.
- Working mode: one patient at a time, or a full ward list in one pass.

If any of this isn't already established:
> "How many patients are we handing over, and do you have notes for each, or
> would you like to talk through them one at a time?"

---

## Step 1: Sort the raw notes into SBAR

For each patient, map whatever was provided into:

- **Situation** — who the patient is, why they're here, current status in
  one line.
- **Background** — relevant history, admission reason, treatment so far.
- **Assessment** — current clinical picture: vitals trend, response to
  treatment, active concerns.
- **Recommendation** — what the incoming shift needs to do, watch for, or
  escalate, and by when.

**Completion criterion:** every patient has content in all four sections, or
an explicit flag on the ones that don't.

---

## Step 2: Flag the gaps

If the source material doesn't cover one of the four sections for a
patient, don't invent it. Mark it clearly instead:

> **[Recommendation not specified — confirm with outgoing shift before
> handover]**

This is the point of the exercise — a handover that silently drops a
missing recommendation is worse than one that visibly flags it.

---

## Step 3: Produce the handover sheet

Output one SBAR block per patient, in the order the outgoing shift will hand
over.

**Completion criterion:** every patient in the list has a labelled SBAR
block, and every flagged gap from Step 2 is visible in the output, not
silently dropped.

---

## Output format

One Markdown block per patient, headed by bed/identifier, with the four SBAR
labels bolded. Keep each section to 1–3 lines — a handover note is a prompt
for the verbal handover, not the full chart.

---

## Gotchas

- This drafts the handover note only. Clinical judgement — what's actually
  urgent, what can wait — stays with the clinicians handing over and
  receiving care.
- Don't paste patient-identifying information beyond what your service's own
  handover process already uses.

---

## Evidence base

- WHO Patient Safety Solutions, *Communication During Patient Hand-Overs*
  (2007) — backs SBAR as the structure, and names incomplete or inconsistent
  handover communication as a leading contributor to preventable harm.
- Institute for Healthcare Improvement, SBAR Tool — the structure this skill
  outputs to.
- ACSQHC, National Safety and Quality Health Service Standards —
  Communicating for Safety standard, backs complete, structured handover as
  an accreditation requirement in Australian health services.
- The Joint Commission, National Patient Safety Goals — handoff
  communication requirement, backs flagging gaps rather than leaving them
  implicit.
