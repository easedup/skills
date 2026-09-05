---
name: patient-letter
version: 1.0.0
released: 2026-09-05
description: >
  Turns clinical or administrative notes into a plain-language letter for a
  patient or family — appointment summary, discharge instructions, results
  explanation, or referral notice — pitched at an accessible reading level
  without dropping any action the patient needs to take. Trigger when a
  clinician or administrator needs to write a patient-facing letter,
  discharge instructions for the patient (not the clinical handover copy),
  or a results letter.
keywords:
  content-type: Patient Communication
  thematic-category: Clinical Communication And Safety
  use-case-theme: Clinical Communication And Safety
  use-case:
    - Patient Correspondence
    - Health Literacy
    - Discharge Communication
  topics: Health Literacy
  keyword:
    - Patient Letter
    - Discharge Instructions
    - Plain Language
    - Results Letter
    - Health Literacy
references:
  - "CDC, Clear Communication Index"
  - "Australian Digital Health Agency"
  - "Agency for Healthcare Research and Quality (AHRQ), Health Literacy Universal Precautions Toolkit"
---

# Patient Letter Writer

A patient letter has done its job only if someone reads it once and knows
exactly what happened and what to do next — regardless of their health
literacy or first language. This skill turns clinical or administrative
notes into a plain-language letter, and treats "what does the patient need
to do" as the one thing that can never get lost in simplification.

This is distinct from a clinical handover note (see `shift-handover-note`)
— that's written for clinicians; this is written for the patient.

---

## What this skill needs

- The letter type: appointment summary, discharge instructions, results
  explanation, or referral notice.
- The clinical/administrative notes to draft from.

If not already clear, ask:
> "What's this letter for, and who's it going to — the patient directly, or
> a family member/carer?"

---

## Step 1: Pull out every required action

Before drafting, list every action the patient needs to take from the
source notes — medication changes, follow-up appointments, warning signs to
watch for, who to contact and when. Nothing patient-facing goes out without
these being explicit.

**Completion criterion:** every action item present in the clinical notes
appears in this list before drafting begins.

---

## Step 2: Draft in plain language

Short sentences, common words, active voice, one idea per sentence. Define
or avoid jargon rather than assuming familiarity. Use "you" directly rather
than passive or third-person clinical phrasing.

**Completion criterion:** no sentence carries more than one instruction or
idea, and no undefined clinical term appears.

---

## Step 3: Close with a clear action list

End with a short "What you need to do" list restating every item from Step
1, plus who to contact with questions and how.

**Completion criterion:** every action from Step 1 appears in this closing
list — none silently dropped for brevity.

---

## Output format

Short paragraphs, then a bulleted "What you need to do" section, then
contact details. Keep to one page where the content allows it.

---

## Gotchas

- This is a draft for the clinician's review before sending, not a
  substitute for their judgement on what to disclose.
- Never soften or omit a safety-relevant instruction (e.g. "seek urgent care
  if X") for the sake of brevity or tone.

---

## Evidence base

- CDC, Clear Communication Index — the plain-language criteria applied in
  Step 2: short sentences, common words, one idea per sentence.
- AHRQ Health Literacy Universal Precautions Toolkit — backs assuming
  variable health literacy for every patient by default, not just those
  flagged as low-literacy, and writing with teach-back-level clarity.
- Australian Digital Health Agency — health literacy guidance for
  Australian patient-facing materials, consistent with the same plain-
  language standard.
