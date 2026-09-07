---
name: read-and-note
description: Records what the user has read, taking their core-claim statement and advancing the note's status, and answers comprehension questions as they read. Use when the user says "I've read this", "I finished the paper", "here are my notes on", "what does this mean" about a source, or asks to check their understanding of a reading.
---

# Read and note

The reading gate is the point of this skill. Enforce it kindly and without
exception.

## The gate

A note advances to `status: read` only when the user has stated, in their own
words:

- the core claim: the author's single main point
- the argument structure: how the author gets there

Ask for both if only one arrives. Do not write these for the user, do not
paraphrase a summary back and call it theirs, and do not advance the status on
"I've read it" alone. If they are stuck, ask questions that help them articulate
it rather than supplying the answer.

When both arrive, write them into the note verbatim as the user wrote them,
set `status: read`, and confirm what this unlocks: the note may now feed
synthesis and draft chapters.

## Quotation verification

To reach `status: verified`, quotations in the note must be checked page by page
against the source, and the user must confirm the check. Where a PDF is
available, locate the passage and report the page; the user still confirms.

## While they read

Expect comprehension questions. Answer them properly: what the term means, why
the author needs it, where it recurs, what an examiner might probe. Add each
explanation to `00-Admin/glossary.md` under a heading naming the term and the
sections it appears in. That file becomes viva preparation.

If a question exposes a genuine problem in the source or the user's reading of
it, say so directly.

## Links

When a note is written or updated, connect it: add `[[wikilinks]]` (or the
equivalent in the user's tool) to the sources it engages, extends or opposes,
with a few words on the relation. Isolated notes are hard to write from later.

## Disagreements between sources

When a new note contradicts an existing one, write the clash to
`30-Contradictions/`: what each source claims, where, and what the argument
turns on. Do not silently pick a winner.
