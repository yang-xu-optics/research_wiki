# Personal Vault — LLM Wiki Schema

This vault is a personal knowledge base built on Andrej Karpathy's **LLM Wiki** pattern
(https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f).

You — the LLM — are the maintainer. The human is the curator, asker, and reader.
Treat this file as the operating contract. When you change a convention here, propagate
the change through existing pages.

---

## Three layers

1. **Raw sources** (`raw/`) — immutable. Articles, papers, gists, transcripts, images.
   You read from `raw/`, you never rewrite a raw file. New sources land in
   `raw/sources/`; images and binaries land in `raw/assets/`.

2. **Wiki** (`wiki/`) — you own this entirely. One file per concept, entity, source
   summary, or overview. Everything is markdown with YAML frontmatter and
   `[[wikilinks]]`.

3. **Schema** (this file, `CLAUDE.md`) — conventions, workflows, and templates.
   Co-evolve it with the human as the vault grows.

Top-level files outside those three layers:

- `index.md` — content-oriented catalog of every wiki page. Updated on every ingest.
- `log.md` — append-only chronological record of ingests, queries, and lints.
- `templates/` — page templates. Copy from here when creating a new page.

---

## Directory layout

```
Personal_Vault/
├── CLAUDE.md              # this file
├── index.md               # content catalog
├── log.md                 # chronological log
├── raw/
│   ├── sources/           # raw inputs, immutable (YYYY-MM-DD-slug.{md,pdf,...})
│   └── assets/            # images, audio, binaries referenced by sources
├── wiki/
│   ├── sources/           # one summary page per raw source
│   ├── entities/          # people, orgs, products, places, tools
│   ├── concepts/          # ideas, methods, terms, patterns
│   └── overviews/         # higher-level syntheses spanning many pages
└── templates/             # page templates
```

---

## Naming conventions

- **Slugs:** `kebab-case`, ASCII, no spaces. Example: `llm-wiki-pattern.md`.
- **Raw sources:** prefix with ingest date: `raw/sources/2026-05-28-karpathy-llm-wiki.md`.
- **Wiki pages:** no date prefix. The slug is the canonical name.
- **People entities:** `firstname-lastname.md` (e.g. `andrej-karpathy.md`).
- **Dates everywhere:** ISO `YYYY-MM-DD`. Convert relative dates ("yesterday") to absolute.
- **Wikilinks:** `[[slug]]` or `[[slug|display text]]`. Bare slug — no `.md`, no folder.
  Obsidian resolves across folders as long as slugs are unique. Keep slugs unique vault-wide.

---

## Page types and frontmatter

Every wiki page starts with YAML frontmatter. Required fields per type below.
Add optional fields freely (Dataview can query anything you put here).

### Source summary — `wiki/sources/<slug>.md`

```yaml
---
type: source
title: "Original title"
authors: [Author Name]
url: https://...
date_published: YYYY-MM-DD          # null if unknown
date_ingested: YYYY-MM-DD
source_file: raw/sources/YYYY-MM-DD-slug.md
kind: article | paper | gist | video | podcast | book | thread | other
tags: [topic1, topic2]
---
```

Body sections (suggested, not enforced): **TL;DR**, **Key claims**, **Notable
quotes**, **Open questions**, **Pages updated by this ingest**.

### Entity — `wiki/entities/<slug>.md`

```yaml
---
type: entity
name: "Display Name"
kind: person | org | product | place | tool | dataset
aliases: []
sources: [[2026-05-28-karpathy-llm-wiki]]
tags: []
---
```

Body: short identity paragraph, then sections relevant to the entity (Role,
Notable work, Positions, Relationships, etc.). Always link out to related
entities and concepts.

### Concept — `wiki/concepts/<slug>.md`

```yaml
---
type: concept
name: "Display Name"
aliases: []
sources: [[2026-05-28-karpathy-llm-wiki]]
related: [[other-concept]]
tags: []
---
```

Body: one-paragraph definition, then **Origin**, **How it works**, **Trade-offs /
Contrasts with**, **Open questions**. Cite sources inline as `[[source-slug]]`.

### Overview — `wiki/overviews/<slug>.md`

```yaml
---
type: overview
title: "Display Title"
scope: "What this overview covers in one sentence"
tags: []
---
```

Body: a synthesis spanning many pages. Heavy on `[[wikilinks]]`. Maintain a
**Last revised** line at the top so staleness is visible.

### Comparison / analysis (filed answer)

Use a `concept`, `overview`, or new `wiki/analyses/<slug>.md` page as fits the
shape. The point: good query answers get filed back. Don't let exploration
disappear into chat.

---

## index.md format

A single markdown file organized by section. Each entry is one line:

```markdown
- [[slug]] — one-line summary
```

Sections, in this order:

1. Overviews
2. Concepts
3. Entities
4. Sources (most recent first)

Update `index.md` on **every** ingest and whenever you create or rename a wiki
page. Keep summaries under ~120 chars.

---

## log.md format

Append-only. Each entry is an H2 with a fixed prefix so it's grep-friendly:

```markdown
## [YYYY-MM-DD] <op> | <title>

- **Source:** [[source-slug]] (only for ingest)
- **Pages touched:** [[page-a]], [[page-b]], ...
- **Notes:** one or two lines on what changed or what was asked.
```

Operations: `ingest`, `query`, `lint`, `refactor`, `note`.

Quick check from a terminal: `grep "^## \[" log.md | tail -10`.

---

## Workflows

### Ingest

When the human drops a new source or points you at one:

1. Save the raw source under `raw/sources/YYYY-MM-DD-<slug>.<ext>`. For web
   articles, prefer markdown via Obsidian Web Clipper; for gists/pages, fetch
   raw and save verbatim.
2. Read it end-to-end. Identify: entities mentioned, concepts introduced,
   claims that contradict or strengthen existing wiki pages.
3. Discuss key takeaways with the human (1-3 sentences). Ask what to emphasize
   only if the framing is ambiguous; otherwise proceed.
4. Create `wiki/sources/<slug>.md` from the source template. Fill TL;DR, key
   claims, quotes worth keeping.
5. For each new entity → create `wiki/entities/<slug>.md` from the entity
   template. For each existing entity → update its page, add the new source to
   its `sources` list, integrate new facts.
6. Same for concepts in `wiki/concepts/`.
7. If the source meaningfully shifts a synthesis, update the relevant
   `wiki/overviews/` page (or create one).
8. Update `index.md` with all new pages.
9. Append a `## [YYYY-MM-DD] ingest | <title>` entry to `log.md` listing every
   page touched.

A single ingest typically touches 5-15 wiki pages. That is normal.

### Query

1. Read `index.md` first to locate candidate pages.
2. Drill into the relevant wiki pages. Follow `[[wikilinks]]` aggressively.
3. Only fall back to raw sources if the wiki page is missing detail or you
   suspect it's stale.
4. Answer with citations as `[[source-slug]]` or `[[page-slug]]`.
5. **File the answer back** if it has lasting value: as a new concept page,
   overview revision, or analysis page. Then update `index.md` and append a
   `query` entry to `log.md`.

### Lint

On request ("lint the wiki"):

- **Contradictions:** scan for pages making opposing claims; flag with a
  `> [!warning]` callout on both pages and a `## Conflicts to resolve` block in
  the lint log entry.
- **Stale claims:** find statements superseded by a newer source (check
  `date_published` in source frontmatter).
- **Orphans:** wiki pages with no inbound `[[wikilinks]]` from any other page.
- **Missing pages:** terms or names cited in 3+ pages without a dedicated page.
- **Broken links:** `[[wikilinks]]` pointing at non-existent slugs.
- **Coverage gaps:** concepts mentioned offhand that deserve their own page;
  suggest sources to find.

Output: a `## [YYYY-MM-DD] lint | <scope>` log entry with the findings as a
checklist. Don't auto-apply destructive changes — propose them.

---

## House rules

- **Wikilinks over prose references.** Every named entity or concept that has a
  page gets `[[linked]]` on first mention in each page.
- **Cite inline.** Claims that came from a source get a trailing `— [[source-slug]]`.
- **Date everything.** Any time-sensitive claim gets an "as of YYYY-MM-DD" tag.
- **No silent rewrites of raw.** `raw/` is read-only. If a source is wrong,
  note it in the source summary page, never edit the raw file.
- **Slugs are forever.** Renaming a slug means updating every inbound
  `[[wikilink]]`. Do the rename in one pass and log it.
- **Don't invent.** If a source doesn't say it, the wiki doesn't claim it.
  Mark uncertain inferences with `?` or "(inferred)".
- **Templates live in `templates/`.** Copy, don't symlink.
- **Auto memory does not belong here.** This vault is the human's, not your
  per-session memory. Keep wiki content domain-content, not meta-notes about
  conversations.
