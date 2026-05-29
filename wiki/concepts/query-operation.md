---
type: concept
name: "Query (operation)"
aliases: ["query"]
sources: [[llm-wiki-pattern-karpathy]]
related: [[llm-wiki-pattern, ingest-operation, lint-operation]]
tags: [workflow]
---

# Query (operation)

> The workflow for asking the wiki a question: read `index.md`, drill into the relevant wiki pages, synthesize an answer with citations — and **file the answer back** if it has lasting value, so exploration compounds — [[llm-wiki-pattern-karpathy]].

## Origin

Defined in the "Operations" section of [[llm-wiki-pattern-karpathy]]. Karpathy stresses the file-back principle: "good answers can be filed back into the wiki as new pages. A comparison you asked for, an analysis, a connection you discovered — these are valuable and shouldn't disappear into chat history."

## How it works

1. Read `index.md` to locate candidate pages.
2. Drill into the relevant wiki pages. Follow `[[wikilinks]]` aggressively.
3. Only fall back to raw sources (`raw/`) if the wiki page is missing detail or you suspect it's stale.
4. Answer with citations: `[[source-slug]]` for source-derived claims, `[[page-slug]]` for wiki-derived ones.
5. If the answer has lasting value, file it back: a new [[concept]] page, an overview revision, or an `analyses/` page. Update `index.md`, append a `query` entry to `log.md`.

## Trade-offs / Contrasts with

- vs [[rag|RAG]] querying — RAG retrieves from raw chunks; the wiki query reads pre-synthesized pages, getting the LLM's prior work for free.
- vs **chat-only** — chat sessions burn the synthesis; wiki querying captures it.

## Open questions

- What threshold of "lasting value" justifies a new page vs leaving the answer in chat? Karpathy doesn't prescribe one.
- Should every query produce a `log.md` entry, or only those that touched wiki pages?

## Related

- [[llm-wiki-pattern]]
- [[ingest-operation]]
- [[lint-operation]]
