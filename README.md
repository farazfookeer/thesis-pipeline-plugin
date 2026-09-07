# Thesis pipeline

A disciplined research and writing pipeline for humanities dissertations at
masters level.

It gives Claude a set of working rules for your project: verify every citation,
never let an unread source into your argument, get editions and translations
right, keep the prose yours, and log what happened so you can declare your AI
use honestly at the end.

Built out of one completed MA dissertation, where it caught inverted claims,
fabricated inferences, a misattributed argument, and several citations that
would not have survived a marker.

## Who it is for

Masters researchers writing an argument-driven dissertation: philosophy,
history, literature, theology, classics, art history, area studies, religious
studies, cultural studies, and interdisciplinary work of the same shape. If your
thesis is defended by reading and reasoning rather than by collected data, this
is built for you.

It assumes no technical knowledge, and it asks your referencing style rather
than imposing one.

## Works where you work

| Your tool | What happens |
|---|---|
| **Obsidian**, Logseq, Roam | The project folder *is* the vault. Notes come with wikilinks, frontmatter properties and theme maps. Nothing to connect. |
| **Notion** or another hosted workspace | Files stay authoritative; the workspace can be mirrored from them if you have that connector. |
| **Word**, Google Docs, **Scrivener** | Draft where you like, export into the drafts folder when you want a check run. |
| **Zotero**, Mendeley, EndNote | Export your PDFs into the sources folder. Citations still get verified independently. |
| **Plain files** | The default. Works with nothing installed. |

## What it does

| Stage | Skill | What happens |
|---|---|---|
| Set up | `set-up-vault` | Creates your folders and records your style, word limit, deadlines and tools |
| Gather | `add-sources` | Turns PDFs into literature notes with citations verified against a named database |
| Primary material | `primary-sources` | Editions, translations, manuscripts, archives, and the locator systems each needs |
| Read | `read-and-note` | Records your reading, enforces the reading gate, answers your questions and builds a glossary |
| Position | `rival-check` | Checks whether anyone has already published your argument |
| Argue | `thesis-log` | Sharpens your thesis through versions and builds a chapter outline with word budgets |
| Write | `revoice` | You rewrite; it checks what your rewriting broke, without touching what it improved |
| Finish | `final-scan` | Word counts, citations both ways, flags, conventions, quotation and edition integrity |
| Declare | `ai-declaration` | Drafts your AI use statement from the actual session record |
| Throughout | `session-log` | Dated entries recording decisions, changes and outstanding flags |

## The rules it holds you to

1. **No citation without provenance.** Nothing gets cited unless its details
   were checked against the source, the publisher, CrossRef, PhilPapers or an
   equivalent. Uncertain sources are marked and excluded from your argument.
2. **No quotation without a locator** - page, folio, Stephanus number, act and
   scene - and your confirmation against the source.
3. **No note counts as read** until you state the core claim in your own words.
   Summaries are reading aids, never substitutes.
4. **Synthesis draws only on what you have read.** Skimmed sources cannot feed
   a chapter.
5. **Editions are part of the citation.** One edition per work, translators
   named, locator systems consistent.
6. **The argument and the prose are yours.** Claude organises, verifies, maps
   and proposes. It does not decide what you think.

## Install

Download `thesis-pipeline.plugin` from the
[latest release](../../releases/latest) and open it in Claude Cowork.

Then see `GETTING-STARTED.md` for step-by-step instructions written for people
who have never installed a plugin. Connector options, all of them optional, are
in `CONNECTORS.md`.

## Contributing

Corrections from other fields are welcome, particularly where a discipline's
citation conventions differ from what is described here. See `CONTRIBUTING.md`.

## Licence

MIT. Use it, change it, share it.
