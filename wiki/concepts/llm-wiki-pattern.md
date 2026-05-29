---
type: concept
name: "LLM Wiki pattern"
aliases: ["LLM wiki", "agent-maintained wiki"]
sources: [[llm-wiki-pattern-karpathy]]
related: [[rag, memex, ingest-operation, query-operation, lint-operation]]
tags: [knowledge-management, pattern]
---

# LLM Wiki pattern

> A pattern for personal knowledge bases in which an LLM agent **incrementally builds and maintains** a persistent, interlinked markdown wiki sitting between the human and the raw sources — rather than re-deriving knowledge from raw chunks on every query as [[rag|RAG]] does — [[llm-wiki-pattern-karpathy]].

## Origin

Proposed by [[andrej-karpathy|Andrej Karpathy]] in a public gist on 2026-05-28 — [[llm-wiki-pattern-karpathy]]. Framed explicitly as a descendant of Vannevar Bush's [[memex]] (1945), with the LLM solving Bush's unsolved problem: who does the maintenance.

## How it works

Three layers:

1. **Raw sources** — immutable inputs (articles, papers, transcripts, images). The LLM reads but never modifies them.
2. **Wiki** — LLM-owned markdown directory: source summaries, entity pages, concept pages, overviews. Heavily cross-linked with `[[wikilinks]]`.
3. **Schema** — a configuration file (e.g. `CLAUDE.md` for [[claude-code|Claude Code]], `AGENTS.md` for Codex) that encodes the conventions and workflows the LLM follows.

Three operations cycle the system:

- **[[ingest-operation|Ingest]]** — absorb a new source, update 10-15 wiki pages.
- **[[query-operation|Query]]** — read the wiki to answer; **file the answer back** if it has lasting value.
- **[[lint-operation|Lint]]** — periodic health-check for contradictions, orphans, stale claims, missing pages.

Two navigation aids:

- `index.md` — content-oriented catalog of every wiki page.
- `log.md` — append-only chronological record; grep-friendly H2 prefix.

## Trade-offs / Contrasts with

- vs [[rag|RAG]] — RAG re-derives on every query (no accumulation, no synthesis carried forward). The wiki pattern accumulates and compounds. RAG scales to millions of docs and arbitrary corpora; the wiki pattern targets the curated, "deep over time" use case.
- vs **plain Obsidian + human author** — same artifact, but the maintenance cost (cross-refs, summaries, consistency) is shifted from the human to the LLM. Karpathy: humans abandon wikis because maintenance grows faster than value.
- vs **chat-only LLM with file uploads** (e.g. [[notebooklm|NotebookLM]]) — those keep raw docs and re-retrieve; exploration disappears into chat history rather than compounding.

## Open questions

- Scaling limits of pure index navigation before [[qmd]]-style hybrid search becomes necessary.
- Schema co-evolution discipline — when and how to revise `CLAUDE.md`.
- Multi-modal handling — images, audio, video in a markdown-first wiki.
- Multi-human collaboration patterns.

## Related

- [[rag]]
- [[memex]]
- [[ingest-operation]]
- [[query-operation]]
- [[lint-operation]]
- [[knowledge-base-architectures]]
