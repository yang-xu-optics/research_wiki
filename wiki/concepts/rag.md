---
type: concept
name: "Retrieval-Augmented Generation (RAG)"
aliases: ["RAG", "retrieval-augmented generation"]
sources: [[llm-wiki-pattern-karpathy]]
related: [[llm-wiki-pattern, notebooklm]]
tags: [llm, retrieval]
---

# Retrieval-Augmented Generation (RAG)

> A pattern where an LLM answers questions by **retrieving relevant chunks** from a raw document collection at query time and generating an answer from them. Knowledge is re-derived on every query; nothing accumulates between questions — [[llm-wiki-pattern-karpathy]].

## Origin

The dominant pattern for "LLM + your documents" workflows: file-upload chats, [[notebooklm|NotebookLM]], embedding+vector-store stacks. Cited by Karpathy as the contrast case motivating the [[llm-wiki-pattern|LLM Wiki pattern]].

## How it works

1. Index raw documents (typically chunked, embedded into a vector store).
2. At query time, retrieve top-k chunks by similarity to the question.
3. Pass retrieved chunks into the LLM's context window as grounding.
4. The LLM generates an answer from those chunks.

## Trade-offs / Contrasts with

- **Strengths:** scales to large, uncurated corpora; minimal setup once indexed; works on read-only docs.
- **Weaknesses (per [[llm-wiki-pattern-karpathy]]):**
  - No accumulation — synthesis across many docs has to be rebuilt every query.
  - No persistent cross-references or contradiction tracking.
  - "Subtle questions" requiring synthesis across 5+ docs are expensive each time.
  - Exploration disappears into chat history.
- vs [[llm-wiki-pattern]] — RAG is stateless across queries; the wiki pattern is stateful and compounding.

## Open questions

- Hybrid setups: at what corpus size does a wiki-pattern KB benefit from layering RAG (or [[qmd]]-style hybrid search) on top of its wiki?
- Can a maintained wiki *replace* RAG up to ~hundreds of sources, as Karpathy claims, in domains beyond text-heavy notes?

## Related

- [[llm-wiki-pattern]]
- [[notebooklm]]
- [[qmd]]
