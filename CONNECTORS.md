# Connectors

## How tool references work

Plugin files use `~~category` as a placeholder for whatever tool you connect in
that category. The pipeline describes workflows in terms of categories rather
than specific products, so it works whatever you use.

## Connectors for this plugin

| Category | Placeholder | Options |
|---|---|---|
| Knowledge base | `~~knowledge base` | Obsidian (files, no connector needed), Notion, Coda, OneNote |
| Reference manager | `~~reference manager` | Zotero, Mendeley, EndNote, Paperpile |
| Document editor | `~~document editor` | Word, Google Docs, Scrivener, LaTeX |

## Nothing is required

The pipeline runs entirely on files in a folder. Connectors are optional
conveniences:

- **Obsidian** needs no connector at all. Point it at your project folder and
  the notes appear, wikilinks and all.
- **Notion** or another hosted workspace can be mirrored from the files if you
  have that connector set up in Cowork. The files stay authoritative.
- **Reference managers** need no connector either. Export your PDFs into the
  sources folder.

If a connector you have named is not available, the plugin says so and carries
on with files rather than stopping.
