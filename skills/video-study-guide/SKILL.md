---
name: video-study-guide
version: 1.0.0
released: 2026-09-13
description: >
  Turns a video transcript into a study guide — a chunked summary, key
  vocabulary, recall and higher-order comprehension questions, and a
  discussion prompt — for pre-viewing preparation or post-viewing
  consolidation. Always flags transcript errors and requires teacher review
  against the actual video before anything reaches students. Trigger when a
  teacher has a video transcript or captions and wants a summary, worksheet,
  or comprehension questions built from it, or asks to turn a video into a
  flipped-classroom task. Does not watch or transcribe video itself — needs
  the transcript text supplied or fetched by whatever capability is
  available in the session.
keywords:
  content-type: Teaching Resource
  thematic-category: Education Objectives And Materials
  use-case-theme: Student Learning And Performance
  use-case:
    - Resource Generation
    - Curriculum & Lesson Planning
    - Personalised Learning
  topics: Video-Based Learning
  keyword:
    - Video Transcript
    - Study Guide
    - Flipped Classroom
    - Comprehension Questions
    - Multimedia Learning
references:
  - "Richard E. Mayer and Logan Fiorella, in The Cambridge Handbook of Multimedia Learning (Cambridge University Press)"
  - "Australasian Journal of Educational Technology (AJET)"
---

# Video Study Guide

You are turning a video transcript into material students or the teacher
can use around the video — not replacing the video itself. A study guide is
only as good as the video and the transcript behind it, so this skill leans
on both honestly rather than presenting a polished-looking output as more
reliable than its source.

---

## Gotchas

- **Transcripts — especially auto-generated captions — contain errors.**
  Technical terms, proper nouns, and numbers are the most error-prone parts
  of any auto-captioned transcript. Flag anything that looks uncertain or
  garbled in the source rather than smoothing it into a confident-sounding
  summary — a wrong number or misheard term repeated in a study guide is
  worse than a gap the teacher has to fill themselves.
- **A study guide doesn't fix a poorly designed video.** Well-designed
  instructional video (chunked, aligned narration and visuals, minimal
  extraneous content) drives real learning gains; principles that improve
  learning in static text don't automatically transfer to video, and this
  skill has no way to assess the video's own design quality from a
  transcript alone. Say so rather than implying the guide guarantees the
  video will teach well.
- **Caption/subtitle evidence is mixed, not uniformly positive.** Captions
  help some learners and some contexts and can hurt others by adding a
  competing text channel to an already-narrated video. Don't blanket
  recommend "turn captions on" as a fix — offer it as one option to trial,
  not a default.
- **Never skip the human-review step.** Everything this skill produces is
  built from a transcript, not a viewing of the video — it must be checked
  against the actual video for accuracy before anything reaches students.

---

## What this skill needs

- The video transcript, subject, and year level. If already known from
  earlier in this conversation, don't ask again.
- Working mode — ask if not already established:
  > "Would you prefer we build this together step by step, or would you
  > like me to produce the full study guide in one pass?"

---

## Step 1: Get the transcript and purpose

Use whatever transcript-retrieval capability is available in this session
if the teacher provides a video link; otherwise ask directly:
> "Paste the transcript or captions for the video. And is this for before
> watching (to prime students for what's coming), after watching (to
> consolidate what they saw), or both?"

Also ask:
> "What subject and year level is this for, and is there a specific focus
> — a particular section, concept, or skill — or should I cover the whole
> video?"

---

## Step 2: Build the study guide

**For pre-viewing:** favour prediction and prior-knowledge questions and a
lighter summary — the point is priming curiosity, not pre-empting the video.

**For post-viewing:** favour a fuller summary and questions that require
students to have actually watched, not ones answerable from the title alone.

---

**VIDEO STUDY GUIDE**

**Video:** [Title/description, as given]
**Subject / Year Level:**
**Use:** [Pre-viewing / Post-viewing / Both]

---

**Summary**
[Chunked by section or timestamp if the transcript has natural breaks —
otherwise 3–5 short paragraphs covering the main content in sequence. Plain
language, no jargon beyond what the video itself introduces.]

*(If any part of the source transcript was unclear or looked like a
transcription error, note it here rather than guessing: "Transcript unclear
around [timestamp/section] — worth checking against the video directly.")*

---

**Key vocabulary**
| Term | Definition (from context) |
|---|---|
| [Term introduced in the video] | [Plain definition] |

---

**Comprehension questions**

*Recall (check they watched and followed):*
1. [Specific, answerable-from-the-video question]
2. [Specific, answerable-from-the-video question]

*Higher-order (check they understood, not just watched):*
1. [Why/how/what-if question requiring synthesis or application, not
   lookup]
2. [Why/how/what-if question]

---

**Discussion prompt**
[One open question connecting the video's content to something students
already know or care about — for class discussion or written reflection]

---

## Step 3: Review reminder

Always close with this, not as a formality:
> "This guide is built from the transcript, not a viewing of the video
> itself — please check it against the actual video before using it with
> students, especially [any flagged uncertain sections] and the technical
> terms in the vocabulary table."

---

## Output format

Deliver the complete study guide in a standalone Markdown code block so the
teacher can copy it directly, or in a dedicated container if building a
larger flipped-classroom task set alongside it. Keep chat text outside the
container brief.

---

## Evidence base
- Mayer, R. & Fiorella, L. (2014), *Cambridge Handbook of Multimedia
  Learning* — backs treating video quality and design as the actual driver
  of learning, not the medium itself; the basis for the "a study guide
  doesn't fix a poorly designed video" gotcha.
  <https://www.cambridge.org/core/books/abs/cambridge-handbook-of-multimedia-learning/principles-for-reducing-extraneous-processing-in-multimedia-learning-coherence-signaling-redundancy-spatial-contiguity-and-temporal-contiguity-principles/CD5B7AE1279A9AB81F8EEBB53DBEC86E>
- Australasian Journal of Educational Technology, *Improving instructional
  video design: A systematic review* — backs the caution that
  design principles proven in static media don't automatically transfer to
  video, and that caption/subtitle effects are mixed rather than uniformly
  positive.
  <https://ajet.org.au/index.php/AJET/article/download/7296/1915/27086>

---

## Step 4: Offer next steps

> "Here's the study guide. Would you like me to turn the comprehension
> questions into a formal exit ticket, build a few diagnostic questions
> around the trickiest concept, or adapt the summary's reading level for
> students who'd find it easier that way?"
