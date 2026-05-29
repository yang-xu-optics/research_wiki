---
type: entity
name: "qmd"
kind: tool
aliases: []
sources: [[llm-wiki-pattern-karpathy]]
tags: [tool, search, on-device]
---

# qmd

> On-device hybrid BM25 / vector search engine for local markdown files, with LLM re-ranking. Recommended in [[llm-wiki-pattern-karpathy]] as the search layer when a wiki grows past the point where `index.md` alone is sufficient.

## Overview

Local search engine purpose-built for markdown vaults. Combines BM25 lexical search with vector similarity and an LLM re-ranking pass. Exposes both a CLI (for shell-out use by an agent) and an MCP server (for native tool use by an LLM).

## Notable work / output

- Hybrid BM25 + vector search over local markdown.
- LLM re-ranking pass over candidates.
- CLI and MCP server interfaces.
- Repository: https://github.com/tobi/qmd

## Relationships

- Optional add-on for the [[llm-wiki-pattern]] as the wiki scales.
- Complements [[obsidian]] vaults specifically (markdown on disk).

## Mentioned in

- [[llm-wiki-pattern-karpathy]] — "qmd is a good option: it's a local search engine for markdown files with hybrid BM25/vector search and LLM re-ranking, all on-device."
