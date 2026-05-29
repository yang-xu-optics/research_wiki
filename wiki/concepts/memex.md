---
type: concept
name: "Memex"
aliases: ["Memex"]
sources: [[llm-wiki-pattern-karpathy]]
related: [[llm-wiki-pattern]]
tags: [history, knowledge-management]
---

# Memex

> Vannevar Bush's 1945 thought-experiment of a personal, curated knowledge store with **associative trails** between documents. The spiritual ancestor of the [[llm-wiki-pattern|LLM Wiki pattern]] — [[llm-wiki-pattern-karpathy]].

## Origin

Proposed by Vannevar Bush in *As We May Think* (1945). Karpathy names it explicitly as the conceptual antecedent: "Bush's vision was closer to this than to what the web became: private, actively curated, with the connections between documents as valuable as the documents themselves."

## How it works (as Bush described)

- A personal device storing a curated library.
- The user creates **associative trails** linking documents — analogous to `[[wikilinks]]`.
- Trails are durable artifacts, shareable and revisitable.

## Trade-offs / Contrasts with

- vs **the web as it actually evolved** — public, uncurated, hyperlinked by authors not readers.
- vs [[llm-wiki-pattern]] — same human-side vision, but with the LLM handling the maintenance burden Bush had no answer for.

## Open questions

- Bush couldn't solve **who does the maintenance**. Karpathy claims the LLM does — but at what scale does even the LLM falter (token costs, drift, hallucination)?

## Related

- [[llm-wiki-pattern]]
