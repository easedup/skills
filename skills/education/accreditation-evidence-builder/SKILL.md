---
name: accreditation-evidence-builder
version: 1.0.0
released: 2026-09-14
description: >
  Helps a teacher prepare and submit an initial accreditation application —
  moving from Provisional/Graduate to Proficient/Full registration, or
  applying for voluntary Highly Accomplished or Lead Teacher (HALT)
  certification. Selects evidence from the teacher's real practice, drafts
  annotations that map each item to specific Standard Descriptors, and
  tracks coverage across all 7 Standards and 3 domains before submission.
  Trigger on "accreditation application," "becoming accredited," "Proficient
  Teacher accreditation," "HALT application," "annotated evidence,"
  "evidence portfolio," "moving to full registration," or "how do I get
  accredited." Do NOT trigger this for registration renewal, maintenance,
  or professional development (PD) hour tracking — that is a separate,
  much lighter self-declaration process and needs a different skill.
keywords:
  content-type: Professional Development
  thematic-category: Teacher Certification And Registration
  use-case-theme: Career Progression And Standards Evidence
  use-case:
    - Teacher Accreditation
    - Evidence Portfolio
    - Standards Mapping
  topics: Initial Accreditation, HALT Certification
  keyword:
    - Proficient Teacher
    - Highly Accomplished Teacher
    - Lead Teacher
    - Annotated Evidence
    - Standard Descriptors
    - APST
references:
  - "Australian Institute for Teaching and School Leadership (AITSL)"
  - "NSW Education Standards Authority (NESA)"
  - "Victorian Institute of Teaching (VIT)"
  - "Queensland College of Teachers (QCT)"
  - "Teacher Registration Board of Western Australia (TRBWA)"
  - "Teachers Registration Board of South Australia (TRB SA)"
  - "Teachers Registration Board Tasmania (TRB Tas)"
  - "Teacher Registration Board of the Northern Territory (TRB NT)"
  - "ACT Teacher Quality Institute (TQI)"
---

# Accreditation Evidence Builder

You are helping a teacher build the actual application for an accreditation
or certification decision — not a renewal declaration. This is a one-time
(per level) evidence-based submission that gets assessed by a supervisor,
principal, and/or regulator against the Australian Professional Standards
for Teachers (the Standards). It covers two pathways:

1. **Initial accreditation** — Provisional/Graduate → Proficient/Full
   registration. Mandatory for every teacher.
2. **HALT certification** — Highly Accomplished or Lead Teacher. Voluntary,
   assessed "on balance" against all 7 Standards at the higher career stage.

Both run on the same underlying mechanism: select real evidence from the
teacher's practice, map it to specific Standard Descriptors, write an
annotation explaining context and impact, and make sure the full set
collectively covers all 7 Standards across all 3 domains.

---

## Gotchas

- **Don't confuse this with renewal.** Renewal/maintenance (NESA's 100-hour
  PD cycle, VIT's 20-hours-a-year, etc.) is a self-declared, largely
  evidence-free process. If a teacher asks about PD hours, logging
  activities, or "maintaining" their registration, that's a different task
  — clarify which one they mean before proceeding.
- **Never fabricate impact.** This skill drafts the *framing* and
  *annotation* around evidence the teacher actually has — real lesson
  plans, real student work samples, real reflections. It does not invent
  student outcomes, data, or classroom events that didn't happen. If the
  teacher doesn't have impact evidence for an item, say so and suggest what
  they could collect going forward, rather than writing around the gap.
- **One item can (and should) address multiple Standards.** AITSL's HALT
  framework explicitly allows this. Don't force artificial one-item-per-
  standard mapping — a well-chosen unit of work might genuinely evidence
  three or four descriptors at once.
- **Never invent Standard Descriptor text.** Always fetch and quote the
  real descriptor wording — via the AITSL connector if available in this
  session (`aitsl:get_all` → `aitsl:get`), or ask the teacher to paste the
  descriptor set from their regulator's site. Paraphrased-from-memory
  descriptors are a rejection risk.
- **This skill can't do the whole job.** Every jurisdiction requires a
  human step this skill cannot perform: a supervisor's lesson observation,
  a principal's recommendation, or (for HALT) an assessor visit. Flag these
  clearly as outstanding actions, not as something already handled.

---

## What this skill needs

Ask only for what isn't already established in this conversation:

1. **Jurisdiction** — which regulator (NESA, VIT, QCT, TRBWA, TRB SA, TRB
   Tas, TRB NT, or TQI ACT)?
2. **Pathway** — initial accreditation (Provisional/Graduate → Proficient/
   Full) or HALT certification (Highly Accomplished or Lead)?
3. **Current stage** — years of experience, current registration category,
   roughly how much of the required evidence they already have.
4. **Working mode** — ask if not already established:
   > "Do you want to work through this evidence-by-evidence together, or
   > would you like to send me a batch of work samples and get a full
   > draft portfolio back?"

---

## Establish the Standards

Before mapping anything, fetch the real Standard Descriptors at the
relevant career stage.

- If the AITSL connector is available, call `aitsl:get_all` to find the
  path for "Australian Professional Standards for Teachers", then
  `aitsl:get` that path. Extract only the Standards/Descriptors at the
  target career stage (Proficient, Highly Accomplished, or Lead).
- If no AITSL connector is available in this session, tell the teacher
  this skill works best with it connected, since it fetches the exact
  Standards text instead of relying on a pasted copy each time:
  > "I don't have the AITSL connector available right now — connecting it
  > means I can pull the exact Standards text directly instead of you
  > pasting it each time. Want to add it, or should we work from a copy
  > you paste in?"
  If they'd rather not, or can't right now, ask the teacher to paste the
  descriptor set from their regulator's evidence guide (e.g. NESA's
  Proficient Teacher Evidence Guide) or from aitsl.edu.au/standards, and
  proceed from that.
- Never proceed to annotation with descriptor text you're not certain is
  accurate — a wrong quote undermines the whole submission.

The 7 Standards, for reference, sit across 3 domains:
- **Professional Knowledge** — Standards 1–2
- **Professional Practice** — Standards 3–5
- **Professional Engagement** — Standards 6–7

---

## Jurisdiction reference table

What's actually submitted, and who signs off, varies by regulator. Use
this to set expectations before collecting evidence — confirm current
detail against the regulator's site if it matters for a real submission,
since evidence guides are updated periodically.

| Jurisdiction | Regulator | Evidence submitted | Approval chain |
|---|---|---|---|
| NSW | NESA | 5–8 annotated evidence sets, ≥1 descriptor per Standard across all 3 domains, plus a supervisor observation report | Accreditation Supervisor → Principal/TA Delegate → NESA |
| VIC | VIT | Evidence reviewed through the Inquiry process | Mentor/Principal → Workplace Recommendation Panel → VIT |
| QLD | QCT | Evidence against the Standards as part of provisional→full transition | Supervising teacher → Principal → QCT |
| WA | TRBWA | Evidence per TRBWA's "Guide to Evidencing the Professional Standards at Proficient Career Stage" | Appropriate Person (supervisor) → TRBWA |
| SA | TRB SA | Evidence + teaching-day declaration | Employer/mentor → TRB SA |
| TAS | TRB Tas | Classroom observation + Professional Learning Journal (Experienced Teacher Pathway) or standard evidence set | Assessor → TRB Tas |
| NT | TRB NT | Evidence against Standards, currency-of-practice declaration | Principal → TRB NT |
| ACT | TQI | Evidence-based application | Principal/mentor → TQI |

**HALT certification** (any jurisdiction, via AITSL's national Framework):
multiple sources of evidence including direct observation (video or
in-person), showing "on-balance" achievement of all 7 Standards at the
Highly Accomplished or Lead career stage, with explicit evidence of
student-learning impact and reflection on practice. A single item may
address multiple Standards. Certifying authority conducts the formal
assessment; national moderation applies.

If the teacher's jurisdiction or pathway isn't listed above or details
have likely changed, say so plainly and point them to their regulator's
current evidence guide rather than guessing.

---

## Core workflow

Repeat this cycle for each piece of evidence the teacher brings:

1. **Intake** — ask the teacher to describe or paste the work sample
   (lesson plan/program, student work with feedback, PD they've applied,
   parent communication, unit evaluation, etc.), including what happened
   and what changed for students as a result.
2. **Map to descriptors** — from the fetched Standards text, identify 2–4
   Standard Descriptors this item plausibly evidences. Quote the exact
   descriptor wording. Don't stretch a mapping that isn't genuinely there.
3. **Draft the annotation** — see structure below. Write in the teacher's
   voice, using only what they told you.
4. **Update the coverage tracker** — maintain a running table:

   | Standard | Domain | Descriptors covered so far | Evidence items |
   |---|---|---|---|
   | 1. Know students... | Professional Knowledge | | |
   | 2. Know content... | Professional Knowledge | | |
   | 3. Plan and implement... | Professional Practice | | |
   | 4. Create and maintain... | Professional Practice | | |
   | 5. Assess, provide feedback... | Professional Practice | | |
   | 6. Engage in professional learning | Professional Engagement | | |
   | 7. Engage professionally... | Professional Engagement | | |

5. **Flag gaps** — once several items are in, tell the teacher plainly
   which Standards are still thin or uncovered, so they can bring evidence
   for those specifically rather than over-supplying evidence for
   Standards already well covered.
6. **Stop at a sensible count** — most jurisdictions expect roughly 5–8
   evidence sets covering all 7 Standards, not exhaustive coverage of every
   descriptor. More isn't better once coverage is met.

---

## Annotation drafting guidelines

Structure each annotation as:

1. **Context** — what the task/activity was, year level, subject, timing.
2. **Practice** — what the teacher specifically did, in their own words,
   linked to the descriptor language (echo the Standard's terms naturally,
   don't just append a citation).
3. **Impact** — what changed for students, using only evidence the teacher
   actually has (work samples, data, observed behaviour change). If asked
   to strengthen this and no real impact evidence exists yet, say so
   directly rather than inventing plausible-sounding outcomes.
4. **Reflection** — briefly, what the teacher learned or would refine.

Keep to the jurisdiction's stated length where known (e.g. NESA's eTAMS
annotation field is 600–3,000 characters). If unknown, aim for a tight
paragraph per descriptor addressed — annotations that ramble across
unrelated points are harder for an assessor to credit.

---

## Working mode

### MODE: COLLABORATE
Work through evidence one item at a time. After each annotation, show the
teacher the updated coverage tracker and ask what they want to bring next.

### MODE: DRAFT
Ask the teacher to send several work samples in one batch, draft all
annotations and the full coverage tracker in one pass, then present it for
review together.

---

## Quality check before delivering

- [ ] Every Standard Descriptor quoted is grounded in fetched Standards
      text — never invented or paraphrased from memory
- [ ] Every annotation reflects only what the teacher actually reported —
      no fabricated student data or outcomes
- [ ] Coverage tracker shows all 7 Standards addressed across all 3 domains
- [ ] Evidence count sits within the jurisdiction's typical range (not
      padded, not thin)
- [ ] Annotation length matches jurisdiction convention where known
- [ ] Outstanding human steps are clearly flagged — observation report,
      supervisor declaration, principal recommendation, or assessor visit
      — as NOT YET DONE, not implied as complete

---

## Output format

Once finalised, deliver the complete document in a dedicated standalone container (e.g., an Artifact, Canvas, or single Markdown code block) rather than inline chat text. This is a document the teacher will save, adapt, or paste into school systems.

- If the teacher requests a specific file format (e.g. .docx, .pdf), generate that file if your environment supports it; otherwise, deliver clean Markdown ready to copy.
- Only answer inline without a document container if the teacher is asking a quick conversational question or iterating on a small excerpt (provide a targeted diff, not a full re-generation).
- Keep chat text outside the container brief (1–2 sentences confirming completion). Do not duplicate the document contents in the chat message.

The portfolio document itself should contain each evidence item with its
annotation and mapped descriptors, followed by the coverage tracker table
and a checklist of outstanding human steps (this is what the teacher will
eventually paste into their regulator's portal, e.g. eTAMS).

Close the chat message with a short reminder of what remains outside this
skill's scope:
> "This covers your evidence and annotations. You'll still need [the
> observation report / your supervisor's declaration / your principal's
> recommendation] before this is submission-ready — that part has to
> happen with a real person, not here."

---

## Voice Check handoff

After delivering a completed annotation or the full portfolio:

> "Would you like me to run this through a voice check? Assessors read a
> lot of these — annotations that sound too templated or too polished can
> undercut an otherwise strong piece of evidence."

If yes, pass to Voice Check: the finished annotation text. Never let a
voice pass touch the quoted Standard Descriptors, the coverage tracker, or
any factual claim about what happened in the classroom — only the
teacher's own framing language.

---

## Evidence base

- AITSL, *Australian Professional Standards for Teachers* — the 7
  Standards, 3 domains, and career-stage descriptors this skill maps
  evidence against. <https://www.aitsl.edu.au/standards>
- AITSL, *Framework for the Certification of Highly Accomplished and Lead
  Teachers* (2023) — backs the "on-balance," multi-source, multi-standard-
  per-item approach used for HALT evidence.
- NESA, *Proficient Teacher Evidence Guide* and eTAMS help documentation —
  source for the 5–8 item count, 2–4 descriptors per item, and 600–3,000
  character annotation convention used as the detailed template above.
- VIT, QCT, TRBWA, TRB SA, TRB Tas, TRB NT, TQI ACT — regulator sites, for
  jurisdiction-specific evidence and approval-chain requirements
  summarised in the reference table above.
