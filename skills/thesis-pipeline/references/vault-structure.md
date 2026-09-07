# Vault structure and templates

## Folders

```
your-project/
  00-Admin/
    project-config.md        settings: referencing style, spelling, word limit, dates
    thesis-log.md            versioned thesis statements and suggestion blocks
    reading-queue.md         dated session log and priority list
    style-profile.md         the author's writing habits, built from their samples
    glossary.md              terms explained during reading, for viva preparation
    supervisor-notes/        meeting notes, emails, feedback
  10-Literature/             one note per source
  20-Maps/                   citation maps, rival checks
  30-Contradictions/         where sources disagree
  40-Outline/                chapter blueprint with word budgets
  50-Sources/                PDFs, named to match their notes
  60-Summaries/              pre-reading extractions (aids, not notes)
  70-Draft/                  chapters, assembled drafts, references, audits
```

## Note template

One file per source in `10-Literature/`, named `AuthorYear-ShortTitle.md`.

```markdown
---
title: "Full title"
authors: "Surname, A. and Surname, B."
year: 2024
citation: "Full reference in the project's style"
doi: "10.xxxx/xxxxx"
source_pdf: "50-Sources/AuthorYear-ShortTitle.pdf"
status: queued        # queued | skimmed | read | verified
provenance: "CrossRef, checked 4 March"
tags: [theme-one, theme-two]
---

## Core claim
(The author's single main claim, in the reader's own words. Required before
status can become `read`.)

## Argument structure
(How they get there, step by step. Required before status can become `read`.)

## Key passages
(Quotations with exact page numbers. Each marked UNVERIFIED until checked
against the PDF.)

## Relevance to my thesis
(What this source does for the argument: supports, complicates, supplies a
method, or is a rival.)

## Questions and doubts
(What is unclear, what to check, what to ask a supervisor.)

## Links
[[Other-Note]] [[Another-Note]]
```

## Status ladder

| Status | Meaning | Who sets it |
|---|---|---|
| `queued` | Identified, not yet obtained or read | Either |
| `skimmed` | Summary generated as a reading aid | Assistant |
| `read` | Author has stated core claim and argument in their own words | Author only |
| `verified` | Quotations checked page by page against the source | Author only |

Only `read` and `verified` notes may feed synthesis or draft chapters.
