---
type: source
title: "LLM Wiki"
authors: [Andrej Karpathy]
url: https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f
date_published: 2026-05-28
date_ingested: 2026-05-28
source_file: raw/sources/2026-05-28-karpathy-llm-wiki.md
kind: gist
tags: [knowledge-management, llm, obsidian, rag, pattern]
---

# LLM Wiki

> [[andrej-karpathy|Karpathy]]'s proposal for a personal knowledge-base pattern where an LLM agent maintains a persistent, structured wiki between the human and their raw sources, instead of re-deriving knowledge from chunks on every query like [[rag|RAG]] does.

## TL;DR

- The LLM **incrementally builds and maintains** a markdown wiki rather than answering from raw chunks. Knowledge is **compiled once, kept current** — a persistent, compounding artifact.
- Three layers: **raw sources** (immutable), **wiki** (LLM-owned markdown), **schema** (`CLAUDE.md` / `AGENTS.md`) that encodes conventions and workflows.
- Three operations: **[[ingest-operation|ingest]]**, **[[query-operation|query]]**, **[[lint-operation|lint]]**. A single ingest typically touches 10-15 wiki pages.
- Two special files: `index.md` (content-oriented catalog) and `log.md` (chronological, grep-friendly).
- The human curates and asks; the LLM does all the bookkeeping — cross-references, summaries, contradiction flags. Karpathy frames it as: "Obsidian is the IDE; the LLM is the programmer; the wiki is the codebase."
- The pattern is intentionally abstract; concrete schema, directory layout, page formats, tooling are left to the implementer + LLM to instantiate.

## Key claims

- Most LLM+document workflows are [[rag|RAG]]-style: re-derive on every query, no accumulation. The wiki pattern accumulates.
- Cross-referencing, contradiction flagging, and consistency are work humans abandon — but cost LLMs near zero, so the wiki stays maintained.
- Index-based navigation (read `index.md` then drill in) works "surprisingly well" up to ~100 sources / hundreds of pages, **without** embedding-based RAG infrastructure.
- Good query answers should be **filed back** into the wiki so exploration compounds, not just ingestion.
- The pattern is spiritually descended from Vannevar Bush's [[memex|Memex]] (1945); the missing piece Bush couldn't solve — who does the maintenance — is now the LLM.
- Use cases span: personal (journaling, goals), research deep-dives, book companion wikis, team/business wikis fed by Slack and transcripts, competitive analysis, trip planning, course notes.

## Notable quotes

> "The LLM is rediscovering knowledge from scratch on every question. There's no accumulation."

> "Obsidian is the IDE; the LLM is the programmer; the wiki is the codebase."

> "The tedious part of maintaining a knowledge base is not the reading or the thinking — it's the bookkeeping."

> "This document is intentionally abstract. It describes the idea, not a specific implementation."

## Open questions

- How well does the index-only navigation scale past ~hundreds of pages before needing [[qmd]] or a real search engine?
- How should the schema (`CLAUDE.md`) co-evolve — versioned in git? Periodically reviewed during lint?
- What is the right cadence for [[lint-operation|lint]]? Per-N-ingests? Time-based?
- How do you handle **multi-modal** sources (images, audio) in a markdown-first wiki? Karpathy notes images are "a bit clunky."
- Is there a clean pattern for **collaborative** wikis (multiple humans, one LLM) — conflict resolution, attribution?

## Pages updated by this ingest

- [[llm-wiki-pattern]] — created; the central concept page
- [[rag]] — created; defined as the contrast pattern
- [[ingest-operation]], [[query-operation]], [[lint-operation]] — created from the gist's "Operations" section
- [[memex]] — created; Bush's 1945 antecedent named in the gist
- [[andrej-karpathy]] — created as the source's author
- [[obsidian]], [[claude-code]], [[notebooklm]], [[qmd]], [[obsidian-web-clipper]], [[marp]], [[dataview]] — created from the tools the gist names
- [[knowledge-base-architectures]] — created as the seed overview for future KB-pattern comparisons
