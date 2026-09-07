---
name: add-sources
description: Adds sources to the dissertation vault with verified citation details, creating a literature note for each. Use when the user says "add these papers", "I've downloaded some PDFs", "add this to my sources", "check this citation", "find the details for this paper", or drops PDFs into the project folder.
---

# Add sources

Turn PDFs or references into literature notes with citations that will survive
a marker's scrutiny.

## Provenance is the whole job

Never write a citation from memory. For each source, establish details from one
of: the PDF's own front matter, the publisher page, CrossRef, PhilPapers,
Semantic Scholar, or the institution's library record. Record which one was used
and when, in the note's `provenance` field.

Where a detail cannot be confirmed, write `[UNVERIFIED]` beside it rather than
a plausible guess. Flag it for the user.

Watch for these, which trip up most drafts:

- Advance-access articles paginated 1-n, later repaginated in an issue
- Electronic-only articles with article numbers rather than page ranges
- Editions and translations of older works, where the year is ambiguous
- Chapters in edited collections, which need both chapter and book details
- Preprints later published under a different title

## Primary or secondary

Mark every note `type: primary` or `type: secondary`. Where the source is
primary - a text under analysis, an edition, a translation, an archival item -
hand off to the `primary-sources` skill, which records the edition and locator
system that its citations will need.

## For each source

1. Read what is available: the PDF if present, otherwise the record.
2. Verify the citation as above.
3. Create `10-Literature/AuthorYear-ShortTitle.md` using the note template from
   the `thesis-pipeline` skill's references, at `status: queued`.
4. Rename the PDF in `50-Sources/` to match the note's filename.
5. If asked, write a reading aid to `60-Summaries/`: overview, structure, key
   passages with page numbers marked UNVERIFIED, and relevance. State clearly at
   the top that this is an aid, not a substitute for reading, and that the note
   cannot advance to `read` on its strength.

## Reference managers and note tools

If the user keeps references in a `~~reference manager`, ask them to export the
PDFs to `50-Sources/` and, if they can, a bibliography file (BibTeX, RIS or CSL
JSON). Read it for details but still verify: reference managers propagate their
users' errors faithfully. Nothing needs connecting; files are enough.

Write notes in the conventions of the user's knowledge tool - wikilinks for
Obsidian and similar, database properties for a hosted workspace. See
`references/knowledge-tools.md` in the `thesis-pipeline` skill.

## Report

List what was added, what was verified and by which source, and anything left
unverified. Then say what is unread and offer `read-and-note`.
