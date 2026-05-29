---
type: overview
title: "Knowledge-base architectures"
scope: "How different patterns organize the relationship between humans, LLMs, and a body of source documents over time"
tags: [knowledge-management, llm, architecture]
---

# Knowledge-base architectures

**Last revised:** 2026-05-28
**Scope:** How different patterns organize the relationship between humans, LLMs, and a body of source documents over time.

> Three broad patterns exist today for "I want an LLM to help me with a growing body of documents." They differ on a single axis: **does anything persist between queries beyond the raw source corpus?** The [[llm-wiki-pattern|LLM Wiki pattern]] proposed by [[andrej-karpathy|Karpathy]] in [[llm-wiki-pattern-karpathy]] is the maximally-persistent end of the spectrum.

## Landscape

- **[[rag|RAG]] / file-upload chat** ([[notebooklm|NotebookLM]], ChatGPT file uploads). Persist only raw documents (often as vector chunks). Re-derive synthesis per query.
- **Plain Obsidian wiki, human-maintained.** Persist a structured wiki, but the human pays the maintenance cost. Karpathy: this is why humans abandon wikis.
- **[[llm-wiki-pattern|LLM Wiki pattern]].** Persist a structured, interlinked wiki *maintained by the LLM*. Synthesis compounds; cross-references stay current; human curates and asks.

## Key axes

- **What persists:** raw only / raw + wiki / raw + wiki + meta-log.
- **Who maintains the structure:** nobody / human / LLM.
- **Scaling lever:** add embeddings (RAG) / add discipline (human wiki) / add agent capacity + optional search like [[qmd]] (LLM Wiki).
- **Where exploration goes:** chat history / scattered notes / filed back into the wiki via [[query-operation]].

## Current thinking

For curated, long-horizon work (deep dives, research, personal KBs of dozens-to-hundreds of sources), the [[llm-wiki-pattern]] looks strictly better than [[rag|RAG]] on every axis except setup cost and corpus size. RAG remains the right tool for uncurated, massive, throw-it-all-in corpora and for one-off Q&A where nothing needs to compound.

The human-only wiki is a degenerate case of the LLM Wiki: same artifact, vastly higher maintenance burden, which is why those wikis decay — per [[llm-wiki-pattern-karpathy]].

## Open threads

- Hybrid stacks: at what wiki size does it make sense to add [[qmd]] or even a RAG layer underneath?
- How does multi-modal content (images, audio, video) change the calculus?
- Are there team/collaborative variants worth tracking separately as the vault grows?
