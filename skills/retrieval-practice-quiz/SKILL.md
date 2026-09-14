---
name: retrieval-practice-quiz
version: 1.0.0
released: 2026-09-13
description: >
  Builds a low-stakes, spaced quiz that deliberately pulls items from
  content taught across several past weeks — not just this lesson — with
  an answer key and corrective feedback for every item, to strengthen
  long-term retention through genuine retrieval effort rather than
  re-reading or re-teaching. Trigger when a teacher wants a review quiz,
  a spaced-practice or interleaved quiz, a way to keep old content fresh,
  or a low-stakes weekly/fortnightly check spanning multiple topics. For a
  single check on today's lesson, an exit ticket fits better; for
  misconception-mapped distractors on one specific concept, a diagnostic
  question bank fits better.
keywords:
  content-type: Assessment
  thematic-category: Education Objectives And Materials
  use-case-theme: Student Learning And Performance
  use-case:
    - Formative Assessment
    - Assessment And Feedback
    - Student Progress Tracking
  topics: Retrieval Practice
  keyword:
    - Retrieval Practice
    - Spaced Practice
    - Interleaving
    - Testing Effect
    - Low-Stakes Quiz
references:
  - "Henry L. Roediger III and Jeffrey D. Karpicke, Perspectives on Psychological Science (Association for Psychological Science)"
  - "Australian Education Research Organisation (AERO)"
---

# Retrieval Practice Quiz

You are building a quiz whose entire purpose is the act of recalling —
not the score. The evidence behind retrieval practice is specific: forcing
genuine, effortful recall from memory (not recognising an answer, not
re-reading notes) is what strengthens long-term retention, and spacing that
recall across time beats massing it all into one review session before a
test.

---

## Gotchas

- **Spacing is what makes this a retrieval-practice quiz, not a review
  quiz.** Deliberately include content from more than one point in the
  past — last week, last month, last term — interleaved rather than
  grouped by topic. A quiz that only tests yesterday's lesson is a recap,
  not spaced retrieval.
- **The recall must be genuine — done away from notes, with no answer
  visible nearby.** If students can look the answer up while answering,
  it's copying, not retrieval. Say this plainly when handing the quiz over.
- **Corrective feedback is not optional.** The benefit of retrieval
  practice depends on students finding out what they got right and wrong,
  ideally straight after attempting it — a quiz with no answer key attached
  loses most of its value. Always include one.
- **Gamification mechanics alone don't guarantee participation or
  learning.** Points, timers, and leaderboards can help engagement, but
  they're a wrapper, not the mechanism — some classes see gamified quiz
  completion collapse well below expectations even with the mechanics in
  place. Treat retrieval effort and feedback as the non-negotiable core,
  and any game-like wrapper as optional and secondary.
- **Keep stakes low.** This is practice, not assessment of learning — avoid
  making it count heavily toward a grade, which pushes students toward
  memorising for the quiz rather than genuine spaced recall.

---

## What this skill needs

- Curriculum, year level, and which topics/weeks to draw content from. If
  already known from earlier in this conversation, don't ask again.
- Working mode — ask if not already established:
  > "Would you prefer we build this together step by step, or would you
  > like me to produce the full quiz in one pass?"

---

## Establish curriculum content

Establish content descriptions for every topic the quiz will draw from —
not just the most recent one. Use whatever curriculum lookup capability is
available in this session; if none is, ask the teacher to name or paste
the relevant content. Never invent content from training data.

---

## Step 1: Plan the spacing

Ask:
> "Which topics should this pull from, and roughly how far back — last
> week, a month ago, last term? A good spaced quiz mixes at least two or
> three different points in time rather than just testing the most recent
> lesson. How many items, and how often will you run this — weekly,
> fortnightly?"

Build the item mix around the answer: allocate more items to
foundational content students need to retain long-term, and fewer to
content that's had less time to fade.

---

## Step 2: Choose the format

> "Short-answer recall questions give the strongest retrieval benefit
> since students have to produce the answer from memory rather than just
> recognise it — but multiple choice is faster to mark at scale and still
> works well if the options are close enough to require real recall, not
> just elimination. Which fits your class better, or would you like a mix?"

---

## Step 3: Generate the quiz

Interleave items across topics — don't block all of one topic's questions
together, since blocking makes the previous item's context inform the
next, reducing genuine independent recall.

---

**RETRIEVAL PRACTICE QUIZ**

**Subject / Year Level:**
**Content spans:** [e.g. "This week's lesson, Week 4's fractions unit, Term 2's measurement unit"]
**Format:** [Short-answer / Multiple choice / Mixed]

1. *[Topic: from N weeks ago]* [Question]
2. *[Topic: from this week]* [Question]
3. *[Topic: from N weeks ago — different topic]* [Question]
*(Continue, interleaving topics rather than blocking them)*

---

**ANSWER KEY AND FEEDBACK**

1. **Answer:** [Correct answer]. [One sentence of corrective feedback — what
   the answer shows, or the most common way to get this wrong and why it's
   wrong]
2. **Answer:** [Correct answer]. [Feedback]
*(Repeat for every item)*

---

## Step 4: Cadence note

Include this with every quiz delivered:
> **Using this well:** Hand back the answer key immediately after students
> attempt it — the retrieval effort matters, but so does finding out
> quickly what stuck and what didn't. Run a version of this regularly
> (weekly or fortnightly) rather than as a one-off, and keep pulling older
> content back in each time rather than only testing what's most recent.

---

## Output format

Deliver the quiz and the answer key as two clearly separated standalone
Markdown code blocks, so the teacher can share the quiz without the
answers visible. Keep conversational text outside the blocks brief.

---

## Evidence base
- Roediger, H.L. & Karpicke, J.D. (2006), *The Power of Testing Memory* —
  the foundational testing-effect finding that effortful retrieval produces
  substantially better long-term retention than re-reading or re-studying;
  the basis for requiring genuine recall away from notes.
  <https://journals.sagepub.com/doi/10.1111/j.1467-9280.2006.01693.x>
- AERO, *Spacing and retrieval practice guide* — backs combining spacing
  and interleaving with retrieval practice, and requiring the retrieval
  attempt to be effortful and followed by feedback for the benefit to hold.
  <https://www.edresearch.edu.au/guides-resources/practice-guides/spacing-and-retrieval-practice-guide-full-publication>

---

## Step 5: Offer next steps

> "Here's the quiz and answer key. Would you like me to build a diagnostic
> question bank for whichever concept the class struggles with most, or
> set up the next quiz already spaced a fortnight ahead?"
