---
name: diagnostic-question-bank
version: 1.0.0
released: 2026-09-13
description: >
  Builds a bank of diagnostic (hinge) multiple-choice questions for a single
  concept, where every wrong answer is mapped to a specific, named
  misconception rather than a throwaway distractor — plus the whole-class
  decision rule for using them (roughly 80% correct, move on; below that,
  re-teach). Trigger when a teacher asks to check for misconceptions, wants
  a hinge question, needs distractors that reveal *why* students got
  something wrong, or asks "what do students usually get wrong about
  [topic]." For a single end-of-lesson check across formats (written,
  discussion, self-assessment), an exit ticket fits better; for spaced
  review of content taught weeks ago, a retrieval-practice quiz fits better.
keywords:
  content-type: Assessment
  thematic-category: Education Objectives And Materials
  use-case-theme: Student Learning And Performance
  use-case:
    - Formative Assessment
    - Assessment And Feedback
    - Student Progress Tracking
  topics: Misconception Diagnosis
  keyword:
    - Hinge Question
    - Diagnostic Question
    - Misconception
    - Distractor Design
    - Formative Assessment
references:
  - "Dylan Wiliam"
  - "Black, P. & Wiliam, D., King's College London (Phi Delta Kappan)"
  - "NSW Department of Education (CESE)"
---

# Diagnostic Question Bank

You are building diagnostic questions — sometimes called hinge questions —
that do more than check whether an answer is right. Every wrong option
exists because a real student would choose it for a real, identifiable
reason. The point isn't just "who got it wrong" — it's "why," and what to
do about it in the next five minutes of the lesson.

An ordinary multiple-choice question with one right answer and three
filler wrong ones tells you a score. A genuine diagnostic question tells
you which misconception to address, and to whom.

---

## Gotchas

- **One concept per question, always.** A question that tests two ideas at
  once makes a wrong answer uninterpretable — you can't tell which of the
  two ideas actually tripped the student up. If the concept has two parts,
  write two questions.
- **A distractor with no real misconception behind it doesn't diagnose
  anything — it just makes the question harder.** If you can't name the
  specific, plausible reasoning that would lead a student to pick an
  option, drop the option. A 3-option question built on three genuine
  misconceptions beats a 4-option question padded with a filler wrong
  answer.
- **The ~80% decision threshold is a practical classroom heuristic, not a
  precisely validated cutoff.** No source backs an exact percentage — teach
  it to the teacher as a rule of thumb they can adjust to their own class,
  not a research-derived number.
- **Answerable in under ~10 seconds, or it isn't a hinge question anymore.**
  If working-out or written justification is needed, it's a good exercise
  but not a diagnostic check — the whole design depends on getting a
  whole-class read in the time it takes to glance at raised hands or clicker
  results.

---

## What this skill needs

- Curriculum, year level, teaching context, and the specific concept to
  diagnose. If already known from earlier in this conversation, don't ask
  again.
- Working mode — ask if not already established:
  > "Would you prefer we build this together step by step, or would you like
  > me to ask a few questions and produce a full set?"

---

## Establish curriculum content

Establish the content description for the concept being diagnosed, using
whatever curriculum lookup capability is available in this session. Never
use training data for curriculum standards — if no lookup capability is
available, ask the teacher to paste the relevant content. This grounds the
question in what students are actually expected to know at this point, not
a generic version of the topic.

---

## Step 1: Identify the concept and its misconceptions

Ask:
> "What specific concept or skill do you want to check — narrow enough that
> one question can test it? And have you noticed particular things students
> get wrong about it, or wrong answers that keep coming up?"

If the teacher names misconceptions they've observed: use these directly —
they're more reliable than anything generated generically, because they're
grounded in this teacher's actual students.

If the teacher hasn't got specific misconceptions in mind: suggest 2–3
common misconceptions associated with this concept, drawing on general
pedagogical content knowledge for the subject — and say plainly that these
are suggestions to confirm or replace, not a diagnosis of this class:
> "Common misconceptions here often include [X], [Y], and [Z] — do any of
> these match what you've seen, or is there a different one you'd rather
> target?"

---

## Step 2: Generate the diagnostic questions

For each confirmed misconception, write one question. Where several
misconceptions relate to the same concept, combine them into a single
question with one distractor per misconception rather than one question
per misconception, so a single 10-second check surfaces all of them at once.

---

**DIAGNOSTIC QUESTION**

**Concept:** [Specific concept being checked]
**Subject / Year Level:**

[Question stem — testable in one read, answerable in under 10 seconds]

A) [Option]
B) [Option]
C) [Option]
D) [Option]

**Answer:** [Correct letter]

**What each option reveals:**
- **[Correct letter]** — Correct. Demonstrates [what understanding this
  shows].
- **[Distractor letter]** — Reveals [specific, named misconception — e.g.
  "believes the sign changes when dividing by a positive number, not just
  a negative one"].
- **[Distractor letter]** — Reveals [specific, named misconception].
- *(Repeat for every distractor. If a plausible misconception can't be
  named for an option, replace or drop it rather than leaving a
  generic "incorrect.")*

---

*(Repeat for each concept the teacher wants to check)*

---

## Step 3: Using the results

Include this note with every set delivered:

> **Using this in class:** Ask the question, get a whole-class response
> (show of hands, mini-whiteboards, or a clicker/polling tool) rather than
> cold-calling one student — the value is in seeing everyone's answer at
> once. As a working rule of thumb, not a precise cutoff: if roughly 80% or
> more answer correctly, the class is ready to move on. Below that, re-teach
> before continuing — and check which wrong answer clustered, since that
> tells you which specific misconception to address, not just that
> re-teaching is needed.
>
> If responses split across two different wrong answers roughly evenly,
> you likely have two different misconceptions in the room needing two
> different explanations, not one re-teach for everyone.

---

## Output format

Deliver each question as its own standalone Markdown code block so the
teacher can copy individual questions rather than the whole set at once.

- Do not wrap the entire bank in a single giant code block.
- Keep conversational text outside the code blocks brief (1–2 sentences
  confirming completion).

---

## Evidence base
- Wiliam, D. — hinge-point questions sit at the intersection of instruction
  and formative assessment, giving a whole-class read frequently enough
  (roughly every 20–30 minutes) to make a real-time teaching decision; the
  basis for this skill's decision-rule note and its 10-second answerability
  requirement.
  <https://arc.educationapps.vic.gov.au/learning/sites/evidence-to-action/10393/Hinge-questions-quick-check-big-impact>
- Black & Wiliam, King's College London (1998), *Inside the Black Box* —
  backs using low-stakes, frequent checks to inform the next teaching move
  rather than only to grade; later meta-analyses find smaller, more
  variable effects than the original synthesis, so treat this as directional
  support rather than a precise figure.
  <http://allianceforlearning.co.uk/wp-content/uploads/2017/03/William-and-Black-Inside-the-Black-Box.pdf>
- NSW DoE/CESE, *What Works Best 2025 — Effective feedback* (2025) — backs
  using the pattern of wrong answers, not just the score, to decide the
  next teaching move.
  <https://education.nsw.gov.au/content/dam/main-education/about-us/educational-data/cese/What_Works_Best_2025_Effective_feedback_practical_guide.pdf>

---

## Step 4: Offer next steps

> "Here's the diagnostic question bank. Would you like me to turn the
> re-teach response into a quick follow-up activity, build an exit ticket
> for the end of the lesson, or put together a retrieval-practice quiz that
> revisits this concept again in a few weeks?"
