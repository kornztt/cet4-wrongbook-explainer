# CET-4 AI 错题讲解助手 — CET-4 Wrong-Question Explainer

A tiny, free, offline-first web app for Chinese university students preparing for CET-4 (College English Test Band 4).

> Honest note: this is a **rule-based explanation engine**, not a generative AI model. It matches pasted questions against a built-in CET-4 grammar/vocabulary rule set and explains the考点, traps, and method step by step. It does not call any API and does not claim to be AI-generated answers.

## Problem Statement

Many CET-4 learners can check whether an answer is right or wrong, but they cannot tell *why*. They repeat the same mistakes because:

1. They do not know which grammar point or vocabulary item a question is testing.
2. They fall for the same distractor patterns (similar words, wrong tense, wrong preposition) again and again.
3. Wrong questions are scattered in notebooks or screenshots, with no spaced review plan.

For students with weak English foundations and limited study time, a heavy app or a paid tutor is not a realistic first step. They need something small, free, and usable in one minute on a phone.

## Solution Overview

A single static web page (`index.html`, no backend, no API key, no build step):

- Paste a CET-4 multiple-choice question → get a structured breakdown: 考点 (tested point), 生词 (key vocabulary), 干扰项陷阱 (distractor traps), 正确思路 (correct method).
- 10 built-in sample questions covering the most common CET-4 patterns: vocabulary, subjunctive mood, emphatic sentences, inversion, tense, fixed collocations, and subject-verb agreement. One click loads and explains each one.
- A wrong-question book saved in `localStorage` (browser only, no upload, no account), with 1 / 3 / 7-day spaced review reminders.

Open `index.html` directly in a browser — it works offline.

## Key Features

- **Rule-based explainer:** pattern matching for `suggest / advise / demand + (should) do`, `not until…that…`, `not only…but also…` (inversion), `be used to doing`, `would rather`, `as if`, `despite / in spite of`, `by the time`, `the number of`, and more.
- **Built-in CET-4 vocabulary notes:** ~30 high-frequency words and collocations (e.g. `abundant`, `compulsory`, `acquire`, `come into effect`, `be allergic to`) with Chinese meanings.
- **10 sample questions:** with answers, tested points, traps, and step-by-step methods.
- **Wrong-book with spaced review:** add a sample or your own question; review dates are auto-set to +1, +3, +7 days, with a “due today” badge.
- **Mobile-friendly, Chinese UI:** English question text, Chinese explanations — the way CET-4 students actually study.

## Technologies Used

- HTML + CSS + vanilla JavaScript (single file, no framework)
- `localStorage` for the wrong-question book
- No backend, no database, no API, no external dependencies

## Target Users

Chinese university students preparing for CET-4, especially those with a weaker English foundation who need a clear, repeatable method for multiple-choice questions — not just an answer key. Also useful for self-study groups and teachers who want a quick classroom demo.

## How to Run

1. Download / clone this project.
2. Open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari, mobile browsers).
3. No installation, no server, no account needed.

## Limitations (honest)

- The explainer is rule-based and covers common CET-4 patterns only; it cannot handle reading-comprehension passages, listening, or writing.
- It does not generate answers for unseen question types — when no pattern matches, it falls back to a general vocabulary/context method.
- Wrong-book data lives only in the browser where it was saved.
