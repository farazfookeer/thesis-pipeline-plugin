# Working with the user's knowledge tool

The vault is a set of folders and markdown files. Most tools either read those
files directly or can be fed from them. Record the user's tool in
`00-Admin/project-config.md` under `Knowledge tool:` and follow the conventions
below.

## Obsidian (and any local markdown tool)

The vault *is* an Obsidian vault. Point Obsidian at the project folder and
everything works with no conversion.

Conventions to follow when writing notes:

- **Wikilinks.** Link notes with `[[AuthorYear-ShortTitle]]`. Add a `## Links`
  section to every literature note listing the sources it engages, agrees with,
  or contradicts. These links are what make the graph view useful.
- **Frontmatter.** Keep the YAML block at the top of each note. Obsidian reads
  `status`, `year`, `tags` as properties and can filter on them.
- **Tags.** Use `tags: [theme-name]` in frontmatter rather than inline `#tags`,
  so themes stay filterable.
- **Maps of content.** For each major theme, write `20-Maps/theme-name.md`
  listing the relevant notes as wikilinks with a sentence on each. This is more
  useful than the graph for actual writing.
- **Dataview.** If the user has the plugin installed, offer a status table:

  ```
  ```dataview
  TABLE status, year FROM "10-Literature" SORT status DESC
  ```
  ```

  Do not assume it is installed. Plain markdown must remain readable without it.

Logseq and Roam work the same way with two differences: they are outline-first,
so keep bullets shallow, and block references (`((block-id))`) can replace
wikilinks where the user prefers them.

## Notion and other hosted workspaces

The vault stays on disk as the working copy. The hosted workspace holds
whatever the user wants visible there.

If a `~~knowledge base` connector is available, offer to mirror:

- A literature database, one row per source, with properties for status, year,
  citation, and provenance
- The reading queue as a log page
- Draft chapters as pages, exported back to markdown for the final assembly

Rules for mirroring:

- The files remain authoritative for word counts, citation checks and the final
  scan. Hosted copies drift; the scan runs on the files.
- Push, do not sync blindly. Ask before overwriting anything the user may have
  edited in the workspace.
- If no connector is configured, say so plainly and carry on with files. The
  pipeline never depends on a connector being present.

## Scrivener and other drafting tools

Some users draft in Scrivener, Word or Google Docs rather than markdown. In that
case:

- Keep notes, sources and admin in the vault as normal
- Let the draft live in the user's tool
- Ask them to export a copy (markdown, .docx or PDF) into `70-Draft/` whenever
  they want a check run on it
- The final scan reads the exported copy and reports issues for the user to fix
  in their own editor

## Zotero, Mendeley, EndNote

Reference managers hold citations; this pipeline holds reading. They coexist:

- Ask the user to export PDFs into `50-Sources/`
- If they can export a bibliography file (BibTeX, RIS, CSL JSON), read it for
  citation details, but still verify against a database or the PDF before use.
  Reference managers propagate their users' errors faithfully.

## Plain files

The default. Folders and markdown, opened in any editor. Everything in this
pipeline works with nothing installed.
