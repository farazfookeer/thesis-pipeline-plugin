# Getting started

Written for researchers, not developers. No technical knowledge needed.

## What you need

- Claude Cowork on your computer
- A folder on your computer for your dissertation
- Your reading as PDFs

That is all. There is nothing to configure and no account to connect. If you use
Obsidian, Notion, Zotero or Scrivener, they fit in - see step 4.

## Step 1: install the plugin

Double-click the `thesis-pipeline.plugin` file, or open Cowork and accept the
plugin when it appears in the chat. You only do this once.

## Step 2: make a folder for your dissertation

Anywhere you like: `Documents/Dissertation` is fine. Leave it empty for now.

## Step 3: connect the folder

In Cowork, choose the folder you just made. Claude can now read and write inside
that folder, and nowhere else.

## Step 4: say what you are doing

Type: **"Set up my dissertation project."**

Claude will ask you eight questions: what your dissertation is about, your
referencing style, British or American spelling, your word limit, your
deadlines, whether your institution has rules about AI use, which tools you work
in, and whether you will be using primary sources such as archives, manuscripts
or translations. Answer them and it builds your folders.

**If you use Obsidian**, open that same folder as a vault when it is built. Your
notes will appear with links between them and a working graph view.

**If you use Notion or similar**, the files stay the master copy and can be
mirrored across if you have that connector set up. Nothing breaks if you do not.

**If you draft in Word, Google Docs or Scrivener**, keep doing that. Export a
copy into the drafts folder whenever you want it checked.

## Step 5: add your reading

Put your PDFs into the `50-Sources` folder that has appeared. Then type:
**"Add these sources."**

Claude will check each paper's citation details against a proper database, write
a note for each one, and tell you about anything it could not verify.

## Step 5b: primary sources

If you are working with a novel, a historical document, scripture, a manuscript
or a translated text, say: **"I'm working with primary sources."**

Claude will ask which edition you have, who translated it, and what reference
system the field uses - Stephanus numbers, folios, act and scene - so that every
citation built on it can be checked. Getting this right at the start saves
rebuilding your references later.

## Step 6: read

Read your sources yourself. This is the part nothing can do for you, and the
plugin will not pretend otherwise.

When you have read one, type: **"I've read the Smith paper."** Claude will ask
you what the core claim is and how the argument works, in your own words. Only
then does the note count as read.

Ask questions while you read. "What does this term mean?" "Why does he need this
example?" Every answer goes into a glossary file, which becomes revision
material for your viva.

## Step 7: work out your argument

Type: **"Help me sharpen my thesis."** Claude proposes versions; you choose and
revise. Then: **"Has anyone already made this argument?"** to check nobody has
published it first.

Then: **"Build my outline."** You get a chapter plan with word budgets.

## Step 8: write

Write your chapters. When you want a check on a passage you have written, paste
it in and say: **"Check this paragraph."**

Claude looks for five things: claims that came out backwards, dropped words like
"only" and "must" that change what you are saying, views attributed to the wrong
person, house style slips, and sentences that make the reader work too hard.

It shows you what it found and waits. Nothing changes in your files until you
say so.

## Step 9: finish

Type: **"Run a final check."** You get word counts, a citation reconciliation in
both directions, any unresolved flags, and a consistency sweep.

Then: **"Draft my AI declaration."** Claude reads the log of everything that
happened during the project and writes an accurate statement of how you used it.
Check it, edit it, submit it.

## A note on honesty

This plugin will not write your dissertation. It refuses to advance a source to
"read" on your say-so alone, it will not invent a citation, and it will tell you
when a sentence you wrote no longer says what you meant.

That is the point. The work stays yours, and the record proves it.

## If something goes wrong

Ask Claude directly: "What stage am I at?" or "What's outstanding?" The project
log in `00-Admin/reading-queue.md` records every session, so you can always pick
up where you left off, even months later.
