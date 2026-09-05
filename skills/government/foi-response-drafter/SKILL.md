---
name: foi-response-drafter
version: 1.0.0
released: 2026-09-05
description: >
  Drafts the structure of a freedom-of-information or public-records
  request response — decision, reasons, exemptions cited, and review
  rights — from case notes and a decision already made, leaving the actual
  release, redaction, and exemption decision to the authorised officer.
  Trigger when an FOI, GIPA, or public-records officer needs to draft a
  decision letter or response to an information request.
keywords:
  content-type: Correspondence
  thematic-category: Public Sector Communications And Governance
  use-case-theme: Public Administration And Accountability
  use-case:
    - Freedom Of Information
    - Records Access
    - Regulatory Correspondence
  topics: Freedom Of Information
  keyword:
    - FOI Response
    - Decision Letter
    - Exemption
    - Review Rights
    - Public Records Request
references:
  - "Office of the Australian Information Commissioner (OAIC), FOI Guidelines"
  - "UK Information Commissioner's Office (ICO), Freedom of Information guidance"
  - "United States Department of Justice, FOIA Guide"
---

# FOI/Public-Records Response Drafter

Name the source, never the decision: this skill needs the officer's actual
release decision — what's released, what's withheld, and which exemption
applies to each withheld item — already made. It never chooses an exemption
or decides what to release; that judgement, including its legal risk, stays
with the authorised decision-maker.

---

## What this skill needs

- The request itself and the items identified as responsive to it.
- For each item: the release decision, and the exemption or ground cited
  for anything withheld.

If the decision inputs aren't present:
> "For each item, what's the release decision, and which exemption or
> ground applies to anything withheld?"

Do not proceed until this is supplied — drafting around a guessed decision
is the failure mode this skill exists to avoid.

---

## Step 1: Confirm the decision is complete

Check that every item identified as responsive has a stated decision and,
where withheld, a named exemption.

**Completion criterion:** no item is missing a release/withhold decision.

---

## Step 2: Draft the letter

Structure: decision summary, item-by-item schedule (with the exemption
cited per withheld item), reasons, and review/appeal rights with the
applicable timeframe.

**Completion criterion:** every withheld item in the draft cites the
exemption the officer specified — never one inferred by this skill.

---

## Step 3: Check completeness

Verify every item in the original request appears in the schedule — either
released or withheld with reasons — and that review rights and their
timeframe are stated.

**Completion criterion:** every item in the request has a decision reflected
in the draft, and review rights appear once, correctly scoped to the
jurisdiction's requirements.

---

## Output format

Decision summary paragraph, item-by-item schedule table (Item | Decision |
Exemption/Reason), review rights paragraph.

---

## Gotchas

- Never selects or infers an exemption on its own — that call belongs
  entirely to the authorised decision-maker.
- This drafts the letter around a decision already made, not the decision
  itself.

---

## Evidence base

- OAIC FOI Guidelines — backs the decision/reasons/exemption/review-rights
  structure required for a valid Australian FOI decision letter.
- UK ICO guidance and US DOJ FOIA Guide — the same structural requirement
  appears in UK and US regimes, backing this as a common shape across
  jurisdictions rather than one-off local practice.
