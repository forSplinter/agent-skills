---
name: learning-record-format
description: Format of the learning records written to ~/learning/records/ at the end of a tutoring session, and read back by the retrieval warm-up.
---

# Learning record format

A **learning record** captures one non-obvious lesson, the way an ADR captures one decision. Write a record only for something that changed how the user thinks, never for a routine fix.

Records live in `~/learning/records/` and are named `NNNN-short-dash-case-title.md`, where the number increments with each record (`0001-join-keys-must-be-unique.md`). Create the folder when it is missing.

Show the user the full record before writing it, and write it only when they confirm. Every sentence in it should sound like them, so reuse their words from the session.

## Template

````markdown
---
title: <one line that states the lesson>
date: <YYYY-MM-DD>
project: <where it happened, or "personal">
next_review: <YYYY-MM-DD>
reviews: 0
---

# 🦦 <title>

> 💡 **The insight**
> <One or two sentences the user could say to a colleague.>

## 🧠 What I believed

<The wrong or incomplete model they started with.>

## ✅ What is actually true

<The corrected model, with a minimal example.>

```<language>
<smallest code or query that shows it>
```

## 🔍 How I got there

<The clue that cracked it, and whether they found it alone, needed a hint or were told.>

## ⚠️ Trap to watch for

<The situation where this will bite again, so they recognise it next time.>

## 🧪 Retrieval question

<One question that tests the lesson by prediction or application.>

<details>
<summary>🦦 Answer</summary>

<The answer, short enough to check in a few seconds.>

</details>

## 🔗 Go deeper

- <Link to the docs page or resource worth reading>
````

## Reviews

The retrieval warm-up updates two fields after asking a record's question.

- When the user answers correctly, increment `reviews` and push `next_review` further out, to 3 days after the first success, then 7, 21 and 60.
- When they get it wrong, reset `reviews` to 0 and set `next_review` to tomorrow.

A record that reaches 60 days with a correct answer is consolidated, and the warm-up can leave it alone.
