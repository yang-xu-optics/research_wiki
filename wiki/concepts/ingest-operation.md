---
type: concept
name: "Ingest (operation)"
aliases: ["ingest"]
sources: [[llm-wiki-pattern-karpathy]]
related: [[llm-wiki-pattern, query-operation, lint-operation]]
tags: [workflow]
---

# Ingest (operation)

> The workflow for absorbing a new raw source into the [[llm-wiki-pattern|wiki]]: read the source, discuss takeaways with the human, write a summary page, update entity and concept pages, append to the log — [[llm-wiki-pattern-karpathy]].

## Origin

Defined in the "Operations" section of [[llm-wiki-pattern-karpathy]]. Karpathy notes a single ingest typically touches **10-15 wiki pages**.

## How it works

In this vault (see [[CLAUDE]] for the exact recipe):

1. Save the raw source under `raw/sources/YYYY-MM-DD-<slug>.<ext>`. Immutable from here.
2. Read end-to-end; identify mentioned entities and introduced concepts.
3. Brief the human on key takeaways (1-3 sentences). Ask for emphasis only if framing is ambiguous.
4. Create `wiki/sources/<slug>.md` from `templates/source.md` — TL;DR, key claims, quotes, open questions.
5. For each entity: create or update `wiki/entities/<slug>.md`. Append source to its `sources` list.
6. For each concept: create or update `wiki/concepts/<slug>.md`.
7. If the synthesis shifts, update or create a `wiki/overviews/<slug>.md`.
8. Update `index.md`.
9. Append a `## [YYYY-MM-DD] ingest | <title>` entry to `log.md` listing every page touched.

## Trade-offs / Contrasts with

- **One-at-a-time** (Karpathy's preference) — human stays in the loop, reads the summary, steers emphasis. Slower, higher quality.
- **Batch ingest** — many sources at once with less supervision. Faster, more drift.
- vs [[query-operation]] — ingest is write-heavy; query is read-heavy and only writes when filing answers back.

## Open questions

- How aggressively to refactor existing pages on ingest vs deferring to [[lint-operation|lint]].
- When does a single source warrant a brand-new [[concept|concept]] page vs a paragraph in an existing one? Rule of thumb: cited in 3+ pages → own page.

## Related

- [[llm-wiki-pattern]]
- [[query-operation]]
- [[lint-operation]]
