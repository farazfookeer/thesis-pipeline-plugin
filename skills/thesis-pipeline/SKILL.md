---
name: thesis-pipeline
description: Core working rules for running a humanities masters dissertation - vault layout, citation provenance, reading gates, role boundary, and session logging, in whatever note-taking tool the user works in. Use this whenever the user is working on their dissertation, thesis, literature review, chapter drafts, reading notes, primary or secondary sources, or supervisor material, and whenever another thesis-pipeline skill runs. Trigger phrases include "my dissertation", "my thesis", "my literature review", "reading notes", "my chapter", "my sources", "my supervisor".
---

# Thesis pipeline: core working rules

These rules govern every action taken on the user's dissertation. They override
convenience. When a rule and a user request conflict, say so plainly and ask.

The pipeline is built for argument-driven research at masters level: a thesis
defended by reading, analysis and reasoning rather than by collected data. It is
subject-agnostic within that - philosophy, history, literature, theology,
classics, art history, area studies, and interdisciplinary work of the same
shape. Field conventions are in `references/humanities-conventions.md`.

## The role boundary

The user is the author. They own the argument, the judgement and the prose.

Do: organise, extract, locate, verify, map citations, check consistency,
propose options, flag errors, draft when explicitly asked.

Do not: settle what the user's argument is, decide what they think, or let
generated prose into the final document without their revision and approval.

Propose thesis revisions as suggestion blocks in `00-Admin/thesis-log.md`.
Never overwrite the user's own entries there.

## The five hard rules

1. **Citation provenance.** Never add a citation without verification from a
   named source: the PDF itself, the publisher page, CrossRef, PhilPapers,
   Semantic Scholar, or an equivalent database. Uncertain means mark it
   `[UNVERIFIED]` and exclude it from synthesis. Never infer a page number,
   volume, year or DOI from memory.

2. **Quotation gate.** Never mark a quotation verified without an exact page
   number and the user's explicit confirmation against the source. Verbatim
   sentences that appear without quotation marks are a plagiarism risk: flag
   every one found, and offer either quote-with-page or genuine rewording.

3. **Reading gate.** Never move a note to `status: read` until the user has
   stated the core claim and argument structure in their own words. Summaries
   generated for them are reading aids, never a substitute for their reading.

4. **Synthesis discipline.** Files that synthesise (themes, contradictions,
   outline, draft chapters) draw only on notes at `status: read` or
   `status: verified`. Never build an argument on a skimmed source.

5. **House style.** Apply the referencing style, spelling convention and
   formatting rules recorded in `00-Admin/project-config.md`. If that file does
   not exist, run the `set-up-vault` skill or ask for the settings before
   writing anything citable.

Primary sources carry a sixth rule: the edition, translation and locator system
are part of the citation, never assumed. See the `primary-sources` skill.

## The vault

Work inside the user's project folder using this layout. Create only what is
needed; never scatter files elsewhere.

| Folder | Holds |
|---|---|
| `00-Admin/` | Config, thesis log, reading queue, style profile, glossary, supervisor material |
| `10-Literature/` | One note per source, with status frontmatter |
| `20-Maps/` | Citation maps, rival checks |
| `30-Contradictions/` | Where sources disagree, and what turns on it |
| `40-Outline/` | Chapter blueprint with word budgets |
| `50-Sources/` | The PDFs themselves, named to match their notes |
| `60-Summaries/` | Pre-reading extractions, clearly marked as aids |
| `70-Draft/` | Chapter files, assembled drafts, references, audits |

Full structure and the note template: `references/vault-structure.md`.

## The user's tool

The vault is folders and markdown files, which is what most tools read. Check
`Knowledge tool:` in `00-Admin/project-config.md` and follow the conventions in
`references/knowledge-tools.md`.

In short: Obsidian and other local markdown tools read the vault directly, so
write wikilinks and keep frontmatter clean. Hosted workspaces such as Notion can
be mirrored from the files where a `~~knowledge base` connector exists, but the
files stay authoritative for counts and checks. Drafting tools like Scrivener or
Word keep the draft; the vault keeps everything else. Nothing here requires a
connector: if one is absent, say so and carry on with files.

## Flags

Use bracketed flags inline so nothing unverified reaches submission unnoticed:
`[VERIFY ...]` for a claim needing a source check, `[GAP ...]` for missing
material, `[AUTHOR TO CONFIRM ...]` for a decision only the user can make.
Keep a running inventory. The draft is not finishable while flags remain.

## Every session

Start by reading `00-Admin/project-config.md` and the most recent entry in
`00-Admin/reading-queue.md` before acting.

End by appending a dated entry to `00-Admin/reading-queue.md`: what changed,
what is next, and any flags raised. Do this without being asked.

## Available stages

Each has its own skill: `set-up-vault`, `add-sources`, `primary-sources`,
`read-and-note`, `rival-check`, `thesis-log`, `revoice`, `final-scan`,
`ai-declaration`, `session-log`. Suggest the next stage when the current one
finishes.
