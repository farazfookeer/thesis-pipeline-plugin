---
name: set-up-vault
description: Sets up a dissertation project folder - creates the vault structure, records the referencing style, word limit and note-taking tool, and starts the reading queue and thesis log. Use when the user says "set up my dissertation", "start my thesis project", "I'm beginning my dissertation", "organise my research folder", or is starting masters research from scratch.
---

# Set up the vault

Create the working structure for a dissertation project. Ask first, build second.

## Ask these questions

Use one form or a short numbered list. Do not proceed on assumptions.

1. What is the dissertation about, in a sentence or two? (Not the final thesis,
   just the territory.)
2. What referencing style does the department require? (Harvard, APA, MLA,
   Chicago, OSCOLA, Vancouver, other.)
3. British or American spelling?
4. What is the word limit, and what does it exclude?
5. What are the key dates: question lock, supervisor deadlines, submission?
6. Is there a supervisor, and does the institution have rules about AI use the
   project must follow?
7. Where do they keep their notes: Obsidian, Notion, Logseq or Roam, a
   reference manager, plain files, or a mix? And where will they write: markdown,
   Word, Google Docs, Scrivener?
8. Will they be working with primary sources - archives, manuscripts, editions,
   translations - or with scholarship alone?

## Then build

Create the folder layout in `references/vault-structure.md` from the
`thesis-pipeline` skill, inside the folder the user has connected.

Write `00-Admin/project-config.md` with the answers:

```markdown
# Project configuration

Field: (subject area)
Referencing style: (style)
Spelling: (British or American)
Word limit: (number), excluding (what)
Key dates:
  - Question lock: (date)
  - Submission: (date)
Supervisor: (name, or none)
Institutional AI policy: (summary, or "to confirm")
Knowledge tool: (Obsidian | Notion | Logseq | Roam | plain files | other)
Drafting tool: (markdown | Word | Google Docs | Scrivener | other)
Reference manager: (Zotero | Mendeley | EndNote | none)
Primary sources: (yes, and of what kind | no)
House rules: (any style bans, e.g. no em-dashes)
```

Then set up for their tool, following `references/knowledge-tools.md` in the
`thesis-pipeline` skill. For Obsidian, tell them to open the project folder as a
vault. For a hosted workspace, check whether the connector exists before
promising to mirror. For a drafting tool, explain that drafts get exported into
`70-Draft/` for checking.

Write `00-Admin/reading-queue.md` with a heading and the first dated entry.

Write `00-Admin/thesis-log.md` with a v0 entry: the research territory as the
user described it, marked "not yet a thesis".

Create the remaining folders empty, each with a one-line `_README.md` saying
what belongs there.

## Close by explaining

Tell the user, in plain language: what was created, where their PDFs go
(`50-Sources/`), how to open it in their tool, and that the next step is
`add-sources` when they have readings, `primary-sources` if they are working
with editions or archives, or `thesis-log` when they want to sharpen the
question.
