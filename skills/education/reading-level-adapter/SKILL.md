---
name: reading-level-adapter
version: 1.0.0
released: 2026-09-13
description: >
  Rewrites a text, passage, or set of instructions to reduce its language
  demand — shorter sentences, higher-frequency vocabulary, defined technical
  terms — while holding the actual content, concept, and cognitive challenge
  fixed. Mapped to the teacher's own curriculum year-level language, never
  to a US grade number. Trigger when a teacher asks to simplify a text,
  lower the reading level, make a passage more accessible, or adapt reading
  material for students who find the language a barrier. For a menu of
  broader support and extension options beyond text itself, a
  differentiation suggester fits better; for scaffolds built specifically
  around a student's home language, a language scaffold builder fits better.
keywords:
  content-type: Teaching Resource
  thematic-category: Education Objectives And Materials
  use-case-theme: Student Learning And Performance
  use-case:
    - Personalised Learning
    - Resource Generation
    - Curriculum & Lesson Planning
  topics: Text Accessibility
  keyword:
    - Reading Level
    - Text Adaptation
    - Adaptive Teaching
    - Vocabulary Load
    - Sentence Complexity
references:
  - "Council of Chief State School Officers"
  - "Ofsted"
  - "Australian Curriculum, Assessment and Reporting Authority (ACARA)"
  - "Australian Institute for Teaching and School Leadership (AITSL)"
---

# Reading Level Adapter

You are rewriting a text so that language is no longer the barrier between a
student and the content — not producing an easier task, a shorter task, or
a lower-expectation version of the same task. The concept, the facts, and
what students are expected to do with them stay exactly as demanding. Only
the language load changes.

---

## Gotchas

- **This produces one resource, not "adaptive teaching."** England's own
  shift from "differentiation" to "adaptive teaching" is about teachers
  reading the room and adjusting live — questioning, feedback, in-the-moment
  scaffolding — not about pre-writing tiered worksheets. A reading-level
  adaptation is raw material a teacher can use *within* adaptive teaching;
  say so, and don't let a request for this turn into "make me three ability
  versions labelled low/medium/high" — that's the exact multi-version
  differentiation pattern the evidence doesn't support.
- **Never simplify away the subject-specific vocabulary that's the actual
  point of the lesson.** If "photosynthesis" is what the lesson teaches,
  keep the word and define it in place — don't replace it with a vaguer
  phrase. Simplify the *surrounding* scaffolding language, not the target
  content itself.
- **A readability score is a surface proxy, not a comprehension guarantee.**
  Formulas built on sentence and word length can rate a genuinely complex,
  well-written text as simple (and vice versa) because they don't measure
  cohesion or the background knowledge a passage assumes. If you compute or
  cite one, label it as a rough indicator to sanity-check by eye, not a
  verdict.
- **Map to this curriculum's own year-level language, never a US grade
  number.** Flesch–Kincaid and Lexile are anchored to the US grade system;
  quoting "Grade 4" to an Australian or UK teacher imports a scale that
  means nothing in their context. Speak in terms of the teacher's own
  curriculum year levels.

---

## What this skill needs

- The source text and the target year level or reading context. If already
  known from earlier in this conversation, don't ask again.
- Working mode — ask if not already established:
  > "Would you prefer we work through this together, or would you like me to
  > produce the full adapted version in one pass?"

---

## Step 1: Get the source text and the barrier

If a text is already in context (e.g. from a lesson plan or student task
sheet produced this session), use it directly.

If standalone:
> "Paste the text you'd like adapted. And what year level or reading
> context is it for?"

Then ask what's actually getting in the way — this shapes what changes:
> "What specifically makes this hard for the students you're thinking of —
> long, complex sentences; unfamiliar vocabulary; or background knowledge
> the text assumes but doesn't explain?"

---

## Step 2: Confirm what must not change

Before rewriting, name what stays fixed:
> "I'll keep the actual content, facts, and the concept exactly as
> demanding — only the language changes. Is there specific vocabulary in
> here that's part of what this lesson is teaching, which I should keep and
> define rather than simplify away?"

---

## Step 3: Adapt the text

Apply changes matched to the barrier identified in Step 1:

**Long or complex sentences:** Break into shorter sentences. Replace
embedded clauses and nominalisations with direct, active-voice statements.
One idea per sentence.

**Unfamiliar vocabulary:** Replace non-essential difficult words with
higher-frequency alternatives. For essential subject-specific terms, keep
the term and add an in-line plain-English definition or a short glossary —
never delete the word the lesson is teaching.

**Assumed background knowledge:** Add a brief explanatory clause or
sentence that supplies the missing context, rather than leaving the gap or
cutting the passage's content down.

Preserve: every fact, every claim, the argument or narrative structure, and
the conceptual demand. The adapted version should be answerable with the
same depth of thinking as the original — a student reading it and a student
reading the original should end up understanding the same thing.

---

**ADAPTED TEXT**

**Source:** [Title/description of original text]
**Subject / Year Level:**
**Adjusted for:** [Sentence complexity / Vocabulary / Background knowledge — whichever applied]

[Adapted text]

**Glossary** *(if technical terms were kept and defined)*
| Term | Plain-English definition |
|---|---|
| [Term] | [Definition] |

---

## Step 4: Show what changed

Before delivering, name the trade-off plainly rather than letting the
teacher discover it:
> "Here's the adapted version. I've kept [specific technical terms] because
> they're what the lesson is teaching, and simplified [what changed —
> sentence length / vocabulary / added context for X]. The content and
> expectation are the same as the original — let me know if anything feels
> like it lost meaning in the process."

If asked for a readability estimate, give one but frame it honestly:
> "As a rough indicator only — formulas like this measure sentence and word
> length, not whether the text actually makes sense to a reader, so treat
> it as a sanity check rather than a target to hit."

---

## Output format

Deliver the adapted text in a standalone Markdown code block so the teacher
can copy it directly. If both the original and adapted versions are useful
side by side for comparison, present them as two clearly labelled blocks.
Keep conversational text outside the blocks brief.

---

## Evidence base
- Council of Chief State School Officers, *Supplemental Information for
  Appendix A of the Common Core State Standards* — backs treating
  Flesch–Kincaid/Lexile-style formulas as surface proxies: they can rate a
  literary classic as suitable for a much younger reader because they
  measure only sentence and word length, not cohesion or assumed knowledge.
  <https://www.thecorestandards.org/wp-content/uploads/Appendix-A-New-Research-on-Text-Complexity-revised.pdf>
- Ofsted, *Research for the Education Inspection Framework* (2019, updated
  2021) — backs distinguishing responsive, in-the-moment adaptive teaching
  from producing multiple pre-written task versions, and treating a single
  adapted text as raw material for the former rather than the whole answer.
  <https://assets.publishing.service.gov.uk/media/6034be17d3bf7f265dbbe2ef/Research_for_EIF_framework_updated_references_22_Feb_2021.pdf>
- ACARA, *EAL/D overview and advice* — backs separating language demand
  from conceptual demand: a student can be held to the same content
  expectation while the language load is adjusted.
  <https://docs.acara.edu.au/resources/EALD_Overview_and_Advice_revised_February_2014.pdf>
- AITSL, Australian Professional Standards for Teachers, Standard 1.5 —
  professional basis for adjusting language demand as a legitimate,
  proactive design choice rather than lowering expectations.
  <https://www.aitsl.edu.au/teach/improve-practice/in-the-classroom/differentiation>

---

## Step 5: Offer next steps

> "Here's the adapted text. Would you like me to build a student task sheet
> around it, generate a vocabulary glossary as a standalone handout, or
> adapt another passage the same way?"
